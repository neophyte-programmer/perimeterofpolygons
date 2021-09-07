#include <iostream>
/*
Printing the perimeter of polygons - Solution Requirements
NB: A polygon is a plane figure that is bounded by a connected
finite number of straight line segments. Example: Pentagon, Hexagon
Create an interactive program to choose the type of polygon,
accept the length of the side in millimeters
Calculate the perimeter of the chosen polygon
Display the name of the polygon, the length of the side,
and the perimeter of the polygon
*/
using namespace std;

int main()
{
    int choice;
    float length, perimeter;
    string name;

    cout << "Choose the type of polygon\n";
    cout << "1. Triangle(3) \n2. Quadrilateral(4) \n3. Pentagon(5)\n";
    cout << "4. Hexagon(6) \n5. Heptagon(7) \n6. Octagon(8)\n";
    cout << "7. Nonagon(9) \n8.Decagon(10) \n9. Hendecagon(11)\n";
    cout << "10. Dodecagon(12)\n" <<endl;
    cin >> choice;

    cout << "Enter the length in mm: ";
    cin >> length;

    switch (choice)
    {
    case 1:
        {
            perimeter = length * 3;
            name = "Triangle";
        }
        break;
    case 2:
        {
            perimeter = length * 4;
            name = "Quadrilateral";
        }
        break;
    case 3:
        {
            perimeter = length * 5;
            name = "Pentagon";
        }
        break;
    case 4:
        {
            perimeter = length * 6;
            name = "Hexagon";
        }
        break;
    case 5:
        {
            perimeter = length * 7;
            name = "Heptagon";
        }
        break;
    case 6:
        {
            perimeter = length * 8;
            name = "Octagon";
        }
        break;
    case 7:
        {
            perimeter = length * 9;
            name = "Nonagon";
        }
        break;
    case 8:
        {
            perimeter = length * 10;
            name = "Decagon";
        }
        break;
    case 9:
        {
            perimeter = length * 11;
            name = "Hendecagon";
        }
        break;
    case 10:
        {
            perimeter = length * 12;
            name = "Dodecagon";
        }
        break;
    default:
        break;
    }

    cout << "\n\n=======================\nName of polygon: " <<name <<endl;
    cout << "Length of side: " <<length <<endl;
    cout << "Perimeter of polygon: " <<perimeter <<"mm" <<endl;
    return 0;
}
