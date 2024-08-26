#include <iostream>
#include <string>

using namespace std;

void listDirectoryContents() {
    cout << "Current directory contains the following files:\n";
    cout << "alpha.txt\nbeta.cpp\nsummary.docx\nimage.jpg\n";
    cout << "Press Enter to return to the menu...\n";
    cin.ignore().get();
}
