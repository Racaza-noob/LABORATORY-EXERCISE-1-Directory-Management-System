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
