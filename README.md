# s1_Karylle-Christiannae-Nicdao
#include <iostream>
using namespace std;

int main() {
	cout << "Please enter your full name." << endl;
	string name, midname, lastname;
	cin >> name >> midname >> lastname;
	cout << "How old are you?" << endl;
	int age;
	cin >> age;
	if (cin.fail()) {
		cin.clear();
		cin.ignore(1000, '\n');
		cout << "Invalid input" << endl;
	}
	else if ((age >= 16) && (age <= 18)) {
		cout << "Would you like to go to the mall? (Y/N)" << endl;
		char ans;
		cin >> ans;
		if ((ans != 'Y') && (ans != 'y') && (ans != 'n') && (ans != 'N')) {
			cout << "Inalid input" << endl;
		}
		else {
			switch (ans) {
			case 'Y':
			case 'y':
				cout << "Enjoy!" << endl;
				break;
			case'N':
			case 'n':
				cout << "Cancelled" << endl;
				break;
			}
		}
	}
	else if ((age == 19) || (age == 21)) {
		cout << "Would you like to go to the theme park? (Y/N)" << endl;
		char ans2;
		cin >> ans2;
		if ((ans2 != 'Y') && (ans2 != 'y') && (ans2 != 'n') && (ans2 != 'N')) {
			cout << "Inalid input" << endl;
		}
		else {
			switch (ans2) {
			case 'Y':
			case 'y':
				cout << "Enjoy!" << endl;
				break;
			case'N':
			case 'n':
				cout << "Cancelled" << endl;
				break;
			}
		}
	}
	else if ((age > 20) && (age <= 25)) {
		cout << "Would you like to go on a trip to Istanbul? (Y/N)" << endl;
		char ans3;
		cin >> ans3;
		if ((ans3 != 'Y') && (ans3 != 'y') && (ans3 != 'n') && (ans3 != 'N')) {
			cout << "Inalid input" << endl;
		}
		else {
			switch (ans3) {
			case 'Y':
			case 'y':
				cout << "Enjoy!" << endl;
				break;
			case'N':
			case 'n':
				cout << "Cancelled" << endl;
				break;
			}
		}
	}
	else if ((age >= 26) && (age <= 30)) {
		cout << "Would you like to go on a trip to Hawaii? (Y/N)" << endl;
		char ans4;
		cin >> ans4;
		if ((ans4 != 'Y') && (ans4 != 'y') && (ans4 != 'n') && (ans4 != 'N')) {
			cout << "Inalid input" << endl;
		}
		else {
			switch (ans4) {
			case 'Y':
			case 'y':
				cout << "Enjoy!" << endl;
				break;
			case'N':
			case 'n':
				cout << "Cancelled" << endl;
				break;
			}
		}
	}
	else if (age == 20) {
		cout << "Would you like to go to the theme park? (Y/N)" << endl;
		char answer;
		cin >> answer;
		if ((answer != 'Y') && (answer != 'y') && (answer != 'n') && (answer != 'N')) {
			cout << "Inalid input" << endl;
		}
		else {
			switch (answer) {
			case 'Y':
			case 'y':
				cout << "Enjoy!" << endl;
				break;
			case'N':
			case 'n':
				cout << "Would you like to take a trip to Istanbul?" << endl;
				char answer2;
				cin >> answer2;
				if ((answer2 != 'Y') && (answer2 != 'y') && (answer2 != 'n') && (answer2 != 'N')) {
					cout << "Inalid input" << endl;
				}
				else {
					switch (answer2) {
					case 'Y':
					case 'y':
						cout << "Enjoy!" << endl;
						break;
					case'N':
					case 'n':
						cout << "Cancelled" << endl;
						break;
					}
				}
			}

		}
	}
	else {
		cout << "I'm sorry, this is for only those aged 16-30." << endl;
	}
}
