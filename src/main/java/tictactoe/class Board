package tictactoe;
public class Board 
{
    int [][] board=new int[3][3];//attributes
    
public void initializeBoard()//method//it use to initialize the board
{
for(int i=0;i<3;i++)
{
for(int j=0;j<3;j++)
{
board[i][j]=2;//Empty=2
}
}
}
public int getBoardValue(int i,int j)//get the value stored in a particular index
{
return board[i][j];
}
public void setBoardValue(int i,int j,int value)//
{
board[i][j]=value;
}
public int possibleWin(int player)//for win possibilities
{
    if(player==1)//player1==x
    {
      for(int i=0;i<3;i++)
      {
       if(board[i][0]*board[i][1]*board[i][2]==18)//for rows
       {
         if (board[i][0]==2)  return i*3+1;//1,4,7
          else if(board[i][1]==2) return i*3+2;//2,5,8
          else return i*3+3;//3,6,9
       }
      }
      for(int j=0;j<3;j++)
      {
       if(board[0][j]*board[1][j]*board[2][j]==18)//for columns
       {
         if (board[0][j]==2)  return j+1;//1,2,3
          else if(board[1][j]==2) return j+4;//4,5,6
          else return j+7;//7,8,9
       }
      }
      if(board[0][0]*board[1][1]*board[2][2]==18)//left diagonal
       {
         if (board[0][0]==2) return 1;
         else if(board[1][1]==2) return 5;
         else return 9;
       }
       if(board[0][2]*board[1][1]*board[2][0]==18)//right diagonal
       {
         if (board[0][2]==2) return 3;
         else if(board[1][1]==2) return 5;
         else return 7;
       }
    }
    else//player2=0
    {
      for(int i=0;i<3;i++)
      {
       if(board[i][0]*board[i][1]*board[i][2]==50)//for rows
       {
         if (board[i][0]==2)  return i*3+1;//1,4,7
          else if(board[i][1]==2) return i*3+2;//2,5,8
          else return i*3+3;//3,6,9
       }
      }
      for(int j=0;j<3;j++)
      {
       if(board[0][j]*board[1][j]*board[2][j]==50)//for columns
       {
         if (board[0][j]==2)  return j+1;//1,2,3
          else if(board[1][j]==2) return j+4;//4,5,6
          else return j+7;//7,8,9
       }
      }
       if(board[0][0]*board[1][1]*board[2][2]==50)//left diagonal
       {
         if (board[0][0]==2) return 1;
         else if(board[1][1]==2) return 5;
         else return 9;
     
       }
       if(board[0][2]*board[1][1]*board[2][0]==50)//right diagonal
       {
         if (board[0][2]==2) return 3;
         else if(board[1][1]==2) return 5;
         else return 7;
       }  
       
    }
     return 0; 
}
public boolean checkWin(int player)//for check, winning status
{
    if(player==1)//player1==x
    {
      for(int i=0;i<3;i++)
      if(board[i][0]*board[i][1]*board[i][2]==27)//for rows
           return true; 
      for(int j=0;j<3;j++)
      if(board[0][j]*board[1][j]*board[2][j]==27)//for columns
           return true;
      if(board[0][0]*board[1][1]*board[2][2]==27)//left diagonal
           return true; 
      if(board[0][2]*board[1][1]*board[2][0]==27)//right diagonal
           return true;
    }
    else//player 2=0
    {
      for(int i=0;i<3;i++)
      if(board[i][0]*board[i][1]*board[i][2]==125)//for rows
           return true; 
      for(int j=0;j<3;j++)
      if(board[0][j]*board[1][j]*board[2][j]==125)//for colunms
           return true;
      if(board[0][0]*board[1][1]*board[2][2]==125)//left diagonal
           return true; 
      if(board[0][2]*board[1][1]*board[2][0]==125)//right diagonal
           return true;     
    }
    return false;
}
public boolean isBoardFilled()
{
    for(int i=0;i<3;i++)
    {
      for(int j=0;j<3;j++)
      {
        if(board[i][j]==2)
        {
          return false;
        }
      }
    }
  return true;
}

   public int randomBlankButton()
    {
     int count=0,s=0;
     for(int i=0;i<3;i++)
    { 
       for(int j=0;j<3;j++)
       {
        if(board[i][j]==2)
        {
         count++;
        }
       }
    }
     int r=1+(int)Math.random()*count;
     for(int i=0;i<3;i++)
      {
       for(int j=0;j<3;j++)
       {
        if(board[i][j]==2)
        { 
        s++;
        }
         if(r==s)
         {
           if(i==0&&j==0) return 1;
           if(i==0&&j==1) return 2;
           if(i==0&&j==2) return 3;
           if(i==1&&j==0) return 4;
           if(i==1&&j==1) return 5;
           if(i==1&&j==2) return 6;
           if(i==2&&j==0) return 7;
           if(i==2&&j==1) return 8;
           if(i==2&&j==2) return 9;
         }
       }
      }
     
     return 0;      
    }


}
