# lab3-practice

#include <iostream> 
int main() {

int gryffindor = 0;
int hufflepuff = 0 ;
int ravenclaw = 0 ;
int slytherin = 0 ;

int ans1, ans2, ans3, ans4;
ans1 = 0;
ans2 = 0;
ans3 =0 ;
ans4 = 0;

std::cout << "The Sorting Hat Quiz!" ;
// -------Question 1--------
std::cout << "Q1) When I'm dead, I want peolpe to remember me as: \n";
std::cout << "1) The Good\n";
std::cout << "2) The Great\n";
std::cout << "3) The Wise\n";
std::cout << "4) The Bold\n";
std::cin >> ans1;

if (ans1 == 1) { 
  hufflepuff = 1 + hufflepuff;
} //if 
else if (ans1 == 2) {
  slytherin = slytherin + 1;
} //else if 1
else if (ans1 == 3){
  ravenclaw = ravenclaw + 1;
} // else if 2
else if (ans1 == 4) {
  gryffindor = 1 + gryffindor;
} // else if 3
else {
std::cout << "Invalid Input";
} // else

//-------Question 2---------
std::cout << "Q2) Dawn or Dusk? \n";
std::cout << "1) Dawn\n";
std::cout << "2) Dusk\n";
std::cin >> ans2;

if (ans2 == 1){
  gryffindor = 1 + gryffindor;
  ravenclaw = 1 + ravenclaw;
} //if

else if (ans2 == 2) {
  hufflepuff = 1 + hufflepuff;
  slytherin = 1 + slytherin;
} // else if 

else {
  std::cout << "Invalid input";
} // else

// --------- Question 3 --------
std::cout << "Q3) Wich kind of instrument most pleases uor ear?\n";
std::cout << "1) The violin\n";
std::cout << "2) The trumpet\n";
std::cout << "3) The piano\n";
std::cout << "4) The drum\n";
std::cin >> ans3;

if (ans3 == 1) { 
  slytherin = 1 + slytherin;
} // if 

else if (ans3 == 2){
  hufflepuff = 1 + hufflepuff;
} // else if 1

else if ( ans3 == 3) {
  ravenclaw = 1 + ravenclaw;
} // else if 2

else if ( ans3 == 4) {
  gryffindor = 1 + gryffindor;
} // else if 3

else {
  std::cout << "Invalid input";
} // else

// ------------ Question 4 ---------------

std::cout << "Q4) Wich roads temps you the most?\n";
std::cout << "1) The wide, sunny grassy lane\n";
std::cout << "2) The narrow, dark, lantern-lit alley\n";
std::cout << "3) The twisting, leaf-steam path trough woods";
std::cout << "4) The cobbled street lined (ancient buildings)\n";
std::cin >> ans4;

if (ans4 == 1){
  hufflepuff = 1 + hufflepuff;
} // if 

else if (ans4 == 2) { 
  slytherin = 1 + slytherin;
} // else if 1

else if (ans4 == 3){ 
  gryffindor = 1 + gryffindor;
} // else if 2

else if (ans4 == 4) {
  ravenclaw = 1 + ravenclaw;
} // else if 3

else {
  std::cout << "Invalid input";
} // else 

// ------ End of questions ----------

std::string house;
int max = 0;

if (gryffindor > max){
  max = gryffindor;
  house = "Gryffindor";
}

if (hufflepuff > max) {
  max = hufflepuff;
  house = "Hufflepuff";
}

if (slytherin > max){
  max = slytherin;
  house = "Slytherin";
}

if (ravenclaw > max){
  max = ravenclaw;
  house = "Ravenclaw";
}

std::cout << house << "!\n";
} //main
