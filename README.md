# Okta-Python-Scripts
Python scripts that demonstrate use of Okta's REST APIs for Unviversal Directory. Description of each script:

1) get_all_active_users_with_app_assignments.py -> Gets all active users and their app assignments to a CSV.
2) get_applications_with_signon_type.py -> Gets all applications and their signon methods to a CSV.
3) deactivate_users_based_on_custom_attribute_value.py -> Deactivates all users in an org with the value of a custom attribute set, then outputs the deactivated users to a CSV.
4) get_assigned_users.py -> Gets all users assigned to a specified application (user ID, user primary email and application username), then outputs the data to a CSV.
5) get_bookmarks_with_usage.py -> Gets all bookmarks and their number of signons by user, then outputs the data to a CSV.
6) get_staged_users.py -> Gets all currently STAGED users in the org, then outputs their data to a CSV.
7) get_swa_with_shared_creds.py -> Gets all active SWA apps with their shared username, then outputs the data to a CSV.

# Requirements to Run Script:

1) Python 2.7 _([Download](https://www.python.org/ftp/python/2.7.14/python-2.7.14.msi))_
2) pip _([Installation Guide](https://pip.pypa.io/en/stable/installing/))_
3) Python's requests libaray (run `pip install requests` from command line or shell)


# How to Run Script

For all scripts open the script in your favorite editor (e.g. Sublime Text 3) and set following variables

1) orgName: including okta/oktapreview to your org e.g. "myorg.okta" or "myorg.oktapreview"
2) apiKey: API token from Okta org (Security -> API -> Token)

If there are any required attribute such as attributeName, triggerValue or appId at the top, update 
those to your needs as well.

In command prompt or shell navigate to folder where Python script is copied "cd ~/Documents/PythonScripts" and run the script e.g
"python get_all_active_users_with_app_assignments.py"


# Credits

Special thanks to Sohaib Ajmal from the Okta Developer Support team who provided the foundation for these scripts.
https://github.com/SohaibAjmal/Okta-UD-Scripts