# Cisco ACI Configuration: Firewall Integration with VRF Sandwich

Example Nexus as Code Configuration files for setting up ACI in a "VRF sandwich" for firewall integration

## Quick Start

- `git clone https://github.com/conmurphy/aci-vrf-sandwich.git`
- `cd aci-vrf-sandwich`
- Update `terraform.tfvars` with your environments details or add the variables as environmental variables
  - `export TF_VAR_aci_url=https://my-apic-url.local`
- `terraform init`
- `terraform plan`
- `terraform apply`

# Notes

- The Terraform code will deploy two tenants with all EPGs, BDs, Contracts, and L3Outs
- It will not configure the L3Domain, AAEP, or VLAN pool
- It is assumed that the ASA and VMware have already been setup
- This scenario is configured to use an ASAv running on UCS connected through Fabric Interconnects

## License

This project is licensed to you under the terms of the [Cisco Sample
Code License](./LICENSE).


