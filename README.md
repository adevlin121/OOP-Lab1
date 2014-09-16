OOP-Lab1
========
void setup()
{
  int i = 0;
  int j = 0;
  int count = 0;
  size(1000, 1000);
  background(0);
  stroke(255, 255, 0);
  fill(0);
  
  for(i=0; i<1000; i=i+100)
  {
    for(j=0; j<1000; j=j+100)
    {
      if(count%2 == 0)
      {
        happy(i, j);
      }
      else
      {
        sad(i, j);
      }
      count++;
    }
    count++;
  }
  
}
void happy(int i, int j)
{
  ellipse((i+50), (j+50), 100, 100);
  ellipse((i+50), (j+50), 8, 8);
  ellipse((i+30), (j+20), 8, 8);
  ellipse((i+70), (j+20), 8, 8);
  line((i+35), (j+70), (i+38), (j+75));
  line((i+38), (j+75), (i+62), (j+75));
  line((i+62), (j+75), (i+65), (j+70));
}

void sad(int i, int j)
{
  ellipse((i+50), (j+50), 100, 100);
  ellipse((i+50), (j+50), 8, 8);
  ellipse((i+30), (j+20), 8, 8);
  ellipse((i+70), (j+20), 8, 8);
  line((i+35), (j+80), (i+38), (j+75));
  line((i+38), (j+75), (i+62), (j+75));
  line((i+62), (j+75), (i+65), (j+80));
}
