Dockstack - Docker Compose Stack Manager

This script checks the status of Docker Compose stacks and allows the user to bring them up or down. It's designed for situations where you have multiple Docker Compose files in various subdirectories, and you want an easy way to manage them.
Usage

Run the script by entering:

bash

./dockstack

The script will list all the Docker Compose stacks it finds in the immediate subdirectories, along with their current status (up or down). It will then ask you to select which files you want to act on.

You can either:

    Enter the numbers corresponding to the files, separated by commas (e.g., 1,3 to select the first and third file), or
    Enter a to select all files.

Next, it will ask what you want to do with the selected files. Enter:

    u to bring the selected stacks up, or
    d to bring the selected stacks down.

Requirements

    Docker
    Docker Compose
    Bash

This script assumes that docker-compose and docker commands are available on your system, and that you have permission to run them.
Limitations

    The script only looks for Docker Compose files (either .yml or .yaml) in the immediate subdirectories of the directory where it's located. It doesn't search recursively in deeper subdirectories.
    The script assumes that Docker Compose files are named docker-compose.yml or docker-compose.yaml. If your compose files have a different name, they won't be found.
