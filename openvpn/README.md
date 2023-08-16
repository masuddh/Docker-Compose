# OpenVPN Client Certificate Generator

This script helps you generate a client certificate and retrieve the corresponding configuration for OpenVPN.

## Prerequisites

- Docker and Docker Compose installed on your system.
- Docker Compose configuration for OpenVPN.

## Usage


1. Clone the [kylemanna/docker-openvpn](https://github.com/kylemanna/docker-openvpn) repository:

    ```
    git clone https://github.com/kylemanna/docker-openvpn.git
    cd docker-openvpn
    ```

3. Follow the instructions in the `kylemanna/docker-openvpn` repository to set up and configure your OpenVPN environment.

4. Back in the `openvpn` directory, make the script executable:

    ```
    chmod +x generate_client.sh
    ```

5. Run the script:

    ```
    ./generate_client.sh
    ```

6. Follow the prompts to provide the client name and choose whether to set a passphrase for the client certificate.

7. The script will generate the client certificate and configuration.

8. Find the client configuration file named `<CLIENTNAME>.ovpn` in the current directory.

9. Connect to your OpenVPN server using the generated client configuration.

## Notes

- If you choose to set a passphrase for the client certificate, you'll be prompted to enter the passphrase when connecting to the VPN.

- If you choose not to set a passphrase, the client certificate will be generated without one.

- Ensure that your OpenVPN Docker Compose environment is properly set up and configured before running this script.

- This script is provided as-is and without warranty. Use it at your own risk.

