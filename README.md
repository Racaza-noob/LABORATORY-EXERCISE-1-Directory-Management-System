#include <iostream>
#include <string>

using namespace std;

void listDirectoryContents() {
    cout << "Current directory contains the following files:\n";
    cout << "alpha.txt\nbeta.cpp\nsummary.docx\nimage.jpg\n";
    cout << "Press Enter to return to the menu...\n";
    cin.ignore().get();
}

void createFolder() {
    cout << "Enter the name for the new folder: ";
    string folderName;
    cin >> folderName;
    cout << "Folder '" << folderName << "' created successfully!\n";
    cout << "Press Enter to return to the menu...\n";
    cin.ignore().get();
}

void changeFolder() {
    cout << "Enter the folder name to navigate to: ";
    string folderName;
    cin >> folderName;
    cout << "You have navigated to: C:\\Users\\YourName\\" << folderName << "\n";
    cout << "Press Enter to return to the menu...\n";
    cin.ignore().get();
}

int main() {
    bool running = true;

while (running) {
        cout << "MAIN MENU\n";
        cout << "1. List Directory Contents\n";
        cout << "2. Create New Folder\n";
        cout << "3. Change Folder\n";
        cout << "4. Exit Program\n";
        cout << "Select an option: ";
        int selection;
        cin >> selection;
        switch (selection) {
            case 1:
                listDirectoryContents();
                break;
            case 2:
                createFolder();
                break;
            case 3:
                changeFolder();
                break;
            case 4:
                running = false;
                break;
            default:
                cout << "Invalid selection! Please choose a valid option.\n";
        }
    }

cout << "Exiting program. Goodbye!\n";
    return 0;
}
