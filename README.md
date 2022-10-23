#include<iostream>
#include<string.h>
#include<cstdlib>

using namespace std;
// _ _1 2_ 0_ _ _
#define  MAX_PASSWORD 2
#define WORD_LENGTH 26
typedef struct
{
	char player_name[20];
	int player_id;
	int current_password;
	int history[WORD_LENGTH];
	double time;
}Player;

Player players[5];

string passwords[MAX_PASSWORD] = {{"REC"}, {"REKA"}};

const char *scenarij1 = 
 "       *  * * * *     \n"
 "       * *      *     \n"
 "       **             \n"
 "       *              \n"
 "       *              \n"
 "       *              \n"
 "       *              \n"
 "      * *             \n"
 "     *   *            \n";
 
const char *scenarij2 = 
 "       *  * * * *     \n"
 "       * *      *     \n"
 "       **      -O-    \n"
 "       *              \n"
 "       *              \n"
 "       *              \n"
 "       *              \n"
 "      * *             \n"
 "     *   *            \n";
 
 const char *scenarij3 = 
 "       *  * * * *     \n"
 "       * *      *     \n"
 "       **      -O-    \n"
 "       *        |     \n"
 "       *        |     \n"
 "       *       /      \n"
 "       *              \n"
 "      * *             \n"
 "     *   *            \n";

 
 const char *scenarij4 = 
 "       *  * * * *     \n"
 "       * *      *     \n"
 "       **      -O-    \n"
 "       *        |     \n"
 "       *        |     \n"
 "       *       / \    \n"
 "       *              \n"
 "      * *             \n"
 "     *   *            \n";
 
 const char *scenarij5 = 
 "       *  * * * *     \n"
 "       * *      *     \n"
 "       **             \n"
 "       *              \n"
 "       *              \n"
 "       *              \n"
 "       *              \n"
 "      * *             \n"
 "     *   *            \n";
 
 const char *scenarij6 = 
 "       *  * * * *     \n"
 "       * *      *     \n"
 "       **             \n"
 "       *              \n"
 "       *              \n"
 "       *              \n"
 "       *              \n"
 "      * *             \n"
 "     *   *            \n";
 
 const char *scenarij7 = 
 "       *  * * * *     \n"
 "       * *      *     \n"
 "       **             \n"
 "       *              \n"
 "       *              \n"
 "       *              \n"
 "       *              \n"
 "      * *             \n"
 "     *   *            \n";
 
 const char *scenarij8 = 
 "       *  * * * *     \n"
 "       * *      *     \n"
 "       **             \n"
 "       *              \n"
 "       *              \n"
 "       *              \n"
 "       *              \n"
 "      * *             \n"
 "     *   *            \n";
 
 const char *scenarij9 = 
 "       *  * * * *     \n"
 "       * *      *     \n"
 "       **             \n"
 "       *              \n"
 "       *              \n"
 "       *              \n"
 "       *              \n"
 "      * *             \n"
 "     *   *            \n";
 
 const char *scenarij10 = 
 "       *  * * * *     \n"
 "       * *      *     \n"
 "       **      -O-    \n"
 "       *     --=|=--  \n"
 "       *        |     \n"
 "       *       / \    \n"
 "       *              \n"
 "      * *  GAME OVER! \n"
 "     *   *            \n";
 

void load_players()
{	
	string name;
	int id;
	Player p;
	
	id = 0;
	for(int i=0;i<5;i++)
	{
		cout <<"Enter player " <<i+1<< " name:"<<endl;
		cin >> name;
		id++;
		p.player_name = name;
		p.player_id = id;
		p.current_password = get_rand_password();
	    p.time = 0;
	    p.current_password = 0;
	    players[i] = p;
	}
}

void display_current_game_state(Player p)
{
	
}

string get_rand_password()
{
	int rand_index = rand() % MAX_PASSWORD; 
	//return passwords[rand_index];
	return rand_index;
}



int main()
{
	cout <<"NANA";
	getchar();
}
