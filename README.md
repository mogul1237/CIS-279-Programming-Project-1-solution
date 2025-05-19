# CIS-279-Programming-Project-1-solution

Download Here: [CIS 279 Programming Project 1 solution](https://jarviscodinghub.com/assignment/cis-279-programming-project-1-solution/)

For Custom/Original Work email jarviscodinghub@gmail.com/whatsapp +1(541)423-7793

This assignment is designed as a review of C++ arrays, class definition and comparison
concepts. These techniques will be used frequently in this course.

PART 1 Code the class described in the specification below. For this class you are to use an array to store the scores in the GolfScore class.

GolfScore Class Specification
// This stores models a golf scorecard. A golf game consists of playing 18 holes of golf, one score per hole. An object of this type stores the 18 scores.

Operations (provided by GolfScore class):
//Effect: initializes all scores to 0
//Precondition: None
//Postcondition: GolfScore object is ready to be used
GolfScore:: GolfScore()

//Effect: new object is a copy of the parameter object
//Precondition: None
//Postcondition: GolfScore object is unchanged
GolfScore::GolfScore(const GolfScore& aCard)

//Effect: adds one stroke for indicated hole number
//Precondition: holeNumber is between 1 and 18, inclusive
//Postcondition: the score for hole number ‘holeNumber’ has been increased by 1
void GolfScore:: add(int holeNumber)

//Effect: deducts one stroke for indicated hole number
//Precondition: None
//Postcondition: if the holdNumber was valid the score for hole number ‘holeNumber’ has been decreased by 1, otherwise a GolfError exception is thrown
* Note: you will need to create a GolfError exception class
void GolfScore:: remove (int holeNumber)

//Effect: determines if the parameter holdNumber is valid (1-18)
//Precondition: None
//Postcondition: No change to GolfScore object
//Returns: true if the holeNumber is valid, false otherwise
bool GolfScore::validHole(int holeNumber) const

//Effect: access method ; provides current score for a particular hold
//Precondition: None
//Postcondition: No change to GolfScore object
//Returns: the current score, if the holdNumber is valid, otherwise a -1 is returned
int GolfScore:: getScore(int holeNumber) const

//Effect: examines two GolfScore objects to determine the winner
//Precondition: scores1 and scores2 GolfScore objects
//Postcondition: both the scores1 and scores2 are unchanged
//Returns: the GolfScore object which has the lowest total score
static GolfScore
GolfScore:: winner (const GolfScore& scores1, const GolfScore& scores2)

//Effect: determines the current score for the entire golf game (sum of all hole scores)
//Precondition: None
//Postcondition: No change to GolfScore object
//Returns: current score of the game
int GolfScore:: total() const

//Effect: determines equality of two GolfScore objects
//Precondition: None
//Postcondition: this GolfScore object is unchanged
//Returns: true if hole scores of calling object are = to that of obj, false otherwise
bool GolfScore::operator== (const GolfScore& obj) const

//Effect: outputs all scores for this GolfScore object in one line, legibly
//Precondition: None
//Postcondition: the GolfScore object is unchanged
//Returns: a the ostream object
friend ostream& operator<<( ostream& out, const GolfScore& obj) //Effect: all scores are reset to 0 //Precondition: None //Postcondition: GolfScore object is like new void GolfScore:: reset() Part 2 Write an application which creates two GolfScore objects and then allows user to repeat any of the following until he/she wishes to exit: (keep in mind preconditions and exception handling) Add a stroke to any hole on GolfScore object 1 (user is prompted for hole#) Add a stroke to any hole on GolfScore object 2 (user is prompted for hole#) Remove a stroke from any hole on GolfScore object 1 (user is prompted for hole#) Remove a stroke from any hole on GolfScore object 2 (user is prompted for hole#) Outputs GolfScore object 1 Outputs GolfScore object 2 Output the score for a particular hole of GolfScore object 1 (user is prompted for hole#) Output the totals for both GolfScore objects, and output the winning card Output a message indicating if GolfScore object1 is equal to GolfScore object 2 Reset both GolfScore objects back to original state Submission Be sure that both your class and your main application are well commented. Each class function should be commented with specification information. The application should have comments indicating what tasks are being performed. Your name should be included in the initial comment for each file that you submit. You are to submit three files only, GolfScore.h, GolfScore.cpp and your main application .cpp file. Submit these files as attachments to an email. Your email should be sent to grassos@smccd.edu, and the subject line should indicate course number and project number. You should receive a ‘thank you’ email within 24 hours of your submission indicating that I have received your project.
