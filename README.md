### Here is a sample script that appends a line to delete_user.yml:

Bash Script to Append a Line
```yaml
#!/bin/bash

# File to modify
PLAYBOOK="delete_user.yml"

# Line to append (this is an example, you can modify it as per your needs)
LINE_TO_APPEND='    - name: Notify user deleted'

# Check if the line is already in the file to avoid duplication
if ! grep -Fxq "$LINE_TO_APPEND" "$PLAYBOOK"; then
  # Append the line to the end of the file
  echo "$LINE_TO_APPEND" >> "$PLAYBOOK"
  echo "Line appended to $PLAYBOOK"
else
  echo "Line already exists in $PLAYBOOK"
fi
```
#### How It Works:

* PLAYBOOK="delete_user.yml": 

Specifies the playbook file you want to append the line to.

* LINE_TO_APPEND='- name: 

Notify user deleted': This is the line that will be appended to the playbook. You can modify this to any content.

* grep -Fxq:

 This checks if the line already exists in the file to avoid appending it multiple times.

* echo "$LINE_TO_APPEND" >> "$PLAYBOOK": 

This appends the line to the playbook if it does not exist.

* How to Run the Script:

Save the above script in a file, for example, append_line.sh.
Make it executable:

chmod +x append_line.sh

* Run the script:

./append_line.sh
This will append the specified line to the delete_user.yml file if it doesn’t already exist.
