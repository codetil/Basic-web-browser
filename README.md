# Basic-web-browser
#!/bin/bash
# Function to open URL in default web browser
open_url() {
xdg-open "$1" }
# Main function to display menu and handle user input
main() {
while true; do
clear
echo "Simple Browser Menu" echo "1. Open Google" echo "2. Open URL" echo "3. Exit"
read -p "Enter your choice: " choice
case $choice in
1)
open_url "https://www.google.com/"
;;
2)
read -p "Enter URL: " url
open_url "$url"
;;
3)
echo "Exiting..." exit 0
;;
*)
echo "Invalid choice. Please try again."
;;
esac
read -p "Press Enter to continue..." done
}
# Run the main function
main
![WhatsApp Image 2024-07-07 at 00 35 50_bd8191bb](https://github.com/codetil/Basic-web-browser/assets/161699300/9a72be92-1443-42e8-ba2a-c21677d8dba2)
