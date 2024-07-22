#!/bin/bash

# Display user information and root status

# Get user ID
user_id=$(id -u)
echo "Your UID is: $user_id"

# Get username
username=$(id -un)
echo "Your username is: $username"

# Check if user is root
if [[ $user_id -eq 0 ]]; then
  echo "You are root"
else
  echo "You are not root"
fi
