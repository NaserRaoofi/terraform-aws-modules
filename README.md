# Terraform Modules

This repository contains a set of reusable Terraform modules designed to simplify and standardize infrastructure deployment across projects. Each module encapsulates best practices and provides configurable resources for common infrastructure components.

## Overview

- **Modular Design:** Each module is self-contained and can be integrated into your Terraform projects as needed.
- **Reusable:** Designed for use across multiple projects to ensure consistency and reduce duplication.
- **Configurable:** Modules expose variables for customization, allowing you to tailor resources to your requirements.

## Structure

- `modules/networking/` - Networking-related resources (VPC, subnets, flow logs, etc.)
- `modules/networking/modules/vpc-endpoints/` - Submodule for VPC endpoints

## Usage

To use a module in your Terraform project, reference it in your configuration:

```hcl
module "networking" {
  source = "github.com/NaserRaoofi/terraform-modules//modules/networking"
  # ... set required variables ...
}
```

Refer to each module's README for specific usage instructions and variable documentation.

## Contributing

Contributions are welcome! Please open issues or submit pull requests for improvements or new modules.

## License

This project is licensed under the MIT License.
