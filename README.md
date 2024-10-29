#include<iostream>
using namespace std;

int main() {
    int k[6] = {3, 8, 1, 4, 6, 7};
    int i = 0;
    int search_element;
    cout << "Enter the search element:" << endl;
    cin >> search_element;

    cout << "Implementation of linear search:" << endl;
    bool found = false; // Flag to check if the element is found

    // Loop until we reach the end of the array
    while (i < 6) {
        if (k[i] == search_element) {
            cout << "The search is successful" << endl;
            cout << "The element found at " << i << " index" << endl;
            found = true; // Set found to true
            break; // Exit the loop
        }
        i++;
    }

    // If the element was not found, inform the user
    if (!found) {
        cout << "Search is unsuccessful" << endl;
    }

    return 0; // Return statement to indicate successful execution
}

