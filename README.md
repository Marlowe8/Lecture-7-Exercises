//Slide 16 (Mark my words)

#include <iostream>
using namespace std;


int Display() {
	int studentGrade = 0;
	cout << "Enter Student's grade: "; cin >> studentGrade;
	return studentGrade;
}

void markGrade(int Grade) {

	if (Grade >= 40 && Grade <= 100) {
		if (Grade >= 70) {
			cout << "Student's mark is: A " << endl;
		}
		else if (Grade >= 60 && Grade <= 69) {
			cout << "Student's mark is: B " << endl;
		}
		else if (Grade >= 50 && Grade <= 59) {
			cout << "Student's mark is: C " << endl;
		}
		else if (Grade >= 40 && Grade <= 49) {
			cout << "Student's mark is: D " << endl;
		}
	}else if (Grade >= 101) {
		cout << "TOO MUCH GRADE!!!" << endl;
	}
	else {
		cout << "Student's mark is: F" << endl;
	}
}

int main() {

	int studentGrade = 0;
	studentGrade = Display();
	markGrade(studentGrade);

	return 0;
}

                                     
                                          
//Slide 17 (Starting a Band)
						      
#include <iostream>
using namespace std;



bool stringTest(string ins) {
	string friendPlaysG = "Guitar", friendPlaysg = "guitar";
	string friendPlaysD = "Drums", friendPlaysd = "drums";


	if (ins == friendPlaysG || ins == friendPlaysg) {
		return true;
	}
	else if (ins == friendPlaysD || ins == friendPlaysd || ins == "drum" || ins == "Drum") {
		return true;
	}
	else {
		return false;
	}

}
void Display() {
	char choice;
	bool musicalFriend = true;
	string instrument;
	while (musicalFriend) {
		cout << "Can you play instrument?\nPress 'y' for yes and Press 'n' for no: "; cin >> choice;
		system("cls");
		if (choice == 'y') {
			cout << "What instrument do you play?: "; cin >> instrument;
			if (stringTest(instrument)) {
				system("cls");
				cout << "cool! you're in, since you can play " << instrument;
				musicalFriend = false;
			}
			else {
				system("cls");
				cout << "Sorry we don't need that at the moment" << endl;
				musicalFriend = false;
			}
		}
		else if (choice == 'n') {
			cout << "You're not for this" << endl;
			musicalFriend = false;
		}
		else {
			cout << "It's not in the choices try again" << endl << endl;
		}
	}
}
int main() {

	Display();

	return 0;
}
	
	
