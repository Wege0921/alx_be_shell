# README

## Description
This repository contains a script to switch the current user to the user `betty`. 

## Requirements
- The script uses exactly 8 characters (+1 character for the new line).
- The user `betty` must exist on the system.

## Instructions

1. **Script Details**
    - The script is named `0-iam_betty`.
    - The purpose of the script is to switch the current user to `betty`.

2. **Usage**
    - Ensure that the user `betty` exists on your system. You can check this by running `id betty` in your terminal.
    - Run the script by executing the following command in your terminal:
      ```sh
      ./0-iam_betty
      ```

3. **Script Content**
    - The content of the script is:
      ```sh
      su betty
      ```

4. **Verification**
    - To verify that the script is exactly 9 characters long, including the newline, you can use the following command:
      ```sh
      tail -1 0-iam_betty | wc -c
      ```
    - This command should output `9`, indicating that the script meets the character requirement.

## Example

1. **Checking User Existence**
    ```sh
    julien@ubuntu:/tmp/h$ id betty
    uid=1001(betty) gid=1001(betty) groups=1001(betty)
    ```

2. **Running the Script**
    ```sh
    julien@ubuntu:/tmp/h$ ./0-iam_betty
    ```

3. **Verifying Script Length**
    ```sh
    julien@ubuntu:/tmp/h$ tail -1 0-iam_betty | wc -c
    9
    ```

## Notes
- Ensure that you have the necessary permissions to switch users on your system.
- This script should be run in a Unix-like environment.

By following the instructions above, you should be able to successfully switch to the user `betty` using the provided script.
