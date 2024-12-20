# Setting the Default Python Version Using `PY_PYTHON` Environment Variable

To set the default Python version using the `PY_PYTHON` environment variable, follow these detailed steps:

## 1. Open the Environment Variables Window
   - Press **Windows key + R** to open the **Run** dialog.
   - Type `sysdm.cpl` and press **Enter**. This opens the **System Properties** window.
   - In the **System Properties** window, go to the **Advanced** tab.
   - Click on the **Environment Variables** button at the bottom.

## 2. Find or Create the `PY_PYTHON` Environment Variable

### If `PY_PYTHON` already exists:
   - Under the **System variables** section, scroll down to find the variable named `PY_PYTHON`.
   - Select `PY_PYTHON` and click on the **Edit** button.
   - Change the **Value** of the variable to the desired Python version (e.g., `3.10`, `3.11`).

### If `PY_PYTHON` doesn't exist:
   - Under the **System variables** section, click on the **New** button.
   - In the **Variable name** field, enter `PY_PYTHON`.
   - In the **Variable value** field, enter the version of Python you want to use as the default (e.g., `3.10`, `3.11`).
   - Click **OK** to save the new variable.

## 3. Apply Changes
   - After editing or creating the `PY_PYTHON` variable, click **OK** on all open dialog boxes to apply the changes.

## 4. Verify the Changes
   - Open a **new Command Prompt** or **PowerShell** window (it’s important to open a new one to ensure the updated environment variable is loaded).
   - Type the following command:

     ```bash
     py --version
     ```

   - This should now launch Python using the version you specified in the `PY_PYTHON` variable (e.g., `3.10` or `3.11`).

## Example: Setting Python 3.10 as Default
If you want to make Python 3.10 the default version:

1. Create or edit the `PY_PYTHON` variable with the value `3.10`.
2. After saving the changes, running `py` in the command prompt will launch Python 3.10 by default.

---

### Additional Notes:
- This process will affect all future uses of `py` in the command prompt, making the version you specify the default version that runs when you type `py`.
- If the `PY_PYTHON` variable is set, it overrides the default version that `py` would normally use.
- If you want to switch back to a different version, you can repeat the process and update `PY_PYTHON` with the desired version.
