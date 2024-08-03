# ppm

`ppm` is a Bash script for executing Python files, capturing output, and sending logs via email. It also includes a man page for usage instructions.

## Installation

1. Clone this repository:

    ```bash
    git clone https://github.com/DanishjeetSingh/ppm.git
    cd ppm
    ```

2. Make the script executable:

    ```bash
    chmod +x ppm
    ```

3. (Optional) Move the script to a directory in your `PATH`. Common directories are `/usr/local/bin` or `~/.local/bin`. For example:

    ```bash
    sudo cp ppm /usr/local/bin/
    ```

4. Install the man page:

    ```bash
    sudo cp ppm.1 /usr/share/man/man1/
    sudo mandb
    ```

## Adding to PATH (Optional)

If you prefer not to move the script, you can add its directory to your `PATH` environment variable:

1. Open your shell's configuration file in a text editor (e.g., `.bashrc`, `.bash_profile`, or `.zshrc`).

    ```bash
    nano ~/.bashrc
    ```

2. Add the following line to the end of the file, replacing `/path/to/ppm` with the actual path to the directory containing your script:

    ```bash
    export PATH="$PATH:/path/to/ppm"
    ```

3. Save the file and reload the shell configuration:

    ```bash
    source ~/.bashrc
    ```

## Usage

To execute the script:

```bash
ppm <python_file> [args...]