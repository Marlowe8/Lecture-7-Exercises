//Slide 16 (Mark my words)

#include <iostream>
using namespace std;


int Display() {
	int studentGrade = 0;
	cout << "Enter Student's grade: "; cin >> studentGrade;
	return studentGrade;
}

void markGrade(int Grade) {

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
 
                                          
                                          
