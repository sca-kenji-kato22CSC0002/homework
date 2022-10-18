# homework

#include <iostream>
#include <cstdlib>
#include <ctime>

using namespace std;

//string answer;
bool answer;

int main() 
{
  srand(static_cast<unsigned int>(time(0)));
  int randomNumber = rand();

  int quesition = (randomNumber %3)+1;

  cout << "問題です" << endl;
    cout << "Oの場合は0\nXの場合は1で答えてください" << endl;

  switch(quesition)
  {
    case 1:
      cout << "車は英語でcarと言う" << endl;
      cin >> answer;

      if (answer == 0)
      {
       cout << "正解です" << endl;
      }
      else
      {
        cout << "不正解です" << endl;
      }
      break;

    case 2: 
      cout << "船は英語でshipと言う" << endl;
      cin >> answer;

      if (answer == 0)
      {
       cout << "正解です" << endl;
      }
      else
      {
        cout << "不正解です" << endl;
      }
      break;

    case 3:
      cout << "船は英語でboatと言う" << endl;
      cin >> answer;

      if (answer == 1)
      {
       cout << "正解です" << endl;
      }
      else
      {
        cout << "不正解です" << endl;
      }
      break;
    }

  return 0;
  }
