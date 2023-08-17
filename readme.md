# SonarQube and Sonar Scanner Installation Automation

This is a base project for automating the installation and configuration of SonarQube and Sonar Scanner on a CentOS 7 virtual machine. Use this project as a starting point to create your own installation automation.

## Requirements

- [Vagrant](https://www.vagrantup.com/downloads)
- [VirtualBox](https://www.virtualbox.org/wiki/Downloads)

## Installing the project

Clone this repository on your machine:

```bash
$ git clone https://github.com/matias96321/lab-vagrant-sonarQube.git
```

Access the project directory:

```bash
$ cd lab-vagrant-sonarQube
```

Start the virtual machine using Vagrant:

```bash
$ vagrant up
```

This will provision a CentOS 7 virtual machine with SonarQube and Sonar Scanner installed.

## Script Details

The `provision.sh` script performs the following steps:

- Creates a user named "sonar".
- Installs essential packages `wget`, `unzip`, and `java-11-openjdk-devel`.
- Downloads and extracts SonarQube and Sonar Scanner distributions.
- Configures a systemd service for SonarQube.
- Adds Sonar Scanner to the system's PATH.
- Installs Node.js.

## Accessing the SonarQube

After executing `vagrant up`, SonarQube will be accessible at `http://localhost:9000` through your web browser.

## Customization

- Replace versions and URLs in the script according to your needs.
- Update installation and usage instructions to fit your project.

## Contribution

Contributions are welcome! Feel free to open issues or submit pull requests.

## License

This project is licensed under the XYZ License. (Replace with the actual license type and corresponding link)
