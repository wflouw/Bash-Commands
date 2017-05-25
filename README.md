# Bash-Commands

Flatten the Folder Structure:
find */ -type f -exec bash -c 'file=${1#./}; echo mv "$file" "${file//\//_}"' _ '{}' \;

Delete Empty Folders:
find */ -depth -type d -exec echo rmdir '{}' \; 

