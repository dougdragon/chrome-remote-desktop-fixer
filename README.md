# Instructions
1. Open PowerShell as administrator
2. Run the following command to see what the current ExecutionPolicy is
     ```bash
     Get-ExecutionPolicy -Scope CurrentUser
     ```
3. Take a note of the current policy
4. Run the following command to allow running PowerShell scripts
    ```bash
    Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
    ```
    - If needed, enter 'Y' to confirm
5. Invoke the CRDFixer.ps1 script:
    ```bash
    CRDFixer.ps1
    ```
6. Run the following to set the ExecutionPolicy back to what it was (change `{ORIGINAL_POLICY}` to whatever was returned in step 2-3 above)
     ```bash
     Set-ExecutionPolicy -ExecutionPolicy {ORIGINAL_POLICY} -Scope CurrentUser
     ```
