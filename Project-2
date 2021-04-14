#include <iostream>
#include <iomanip>
using namespace std;
int main()
{
    int numComputers = 0;
    int hightPerf = 0;
    int lowPerf = numeric_limits <int>::max ();

    // Variable to store low performsnce value initialized to infinity do

    {
        cout << " How many compuerts are being proccessed? ";
        cin >> numComputers;

        if (numComputers < 1)
        {
            cout << " Value should not be less than 1. Please try again.\n';                         
        }
    } while (numComputers < 1);

    // step 2
     cout << "\n\nComputer Hardware Graphics Quality Recommendation Tool\n\n " ;

    // step 3
    while (numComputers >0)
    {
        int choice;
        int clkspGPU ;
        int numCores ;

        // step 4
        cout << " Please enter the cloc speed (in Megahertz) of your Graphic card: " ;
        cin >> clkspGPU ;

        if ( clkspGPU < 800 || clkspGPU > 200)
        {
            cout << " GPU clock speed should lie between 800 (inclusive) and 2000 MHz (inlcusive). Please try again.\n" ;

        } while (clkspGPU < 800 || clkspGPU > 2000);

        // step 4
        do
        cout << " Please enetr the clock speed (in Megahertz) of your processor: " ;
        cin >> clkspGPU;

        if(clkspCPU < 1000 || clkspCPU > 5500)
        {
            cout << "CPU clock speed should lie between 1000 (inclusive) and 5500 MHz (inclusive). Please try again.\n" ;

        } while (clkspCPU < 1000 || clkspCPU > 5500);

        //step 4
        do
        cout << "Please enter the number of cores of your processor: ";
        cin >> numCores;

        if(numCores <1 || numCores > 16)
        cout << "Number of Cores ahould lie between 1 (inclusive) and 16 (inclusive). Plaese try again.\n";

        while (numCores <1 || numCores > 16) ;

        const int Low = 1,
        Mid = 2,
        High = 3,
        Higest = 4 ;

        do
        {
            cout << "What is the resolution of your monitor? " ;
            << "\t1. 1280 * 720 \n"
            << "\t2. 1920 * 1080 \n"
            << "\t3. 2560 * 1440 \n"
            << "\t4. 3840 * 2160 \n"
            << "Please select from the options above: " ;
            cin >> choice;

            if (choice < 1 || choice >4 )
            cout << "Select a value between 1 (inclusive) and 4 (inclusive). Please try again.\n";
        
        } while(choice < 1 || choice > 4);

            if (choice ==1)
            {
                multiplier =1 ;
            }
            else if (choice == 2)
            {
                multiplier = 0.55 ;
            }
            else
            {
                multiplier = 0.35 ;
            }

        }

        // Calculate performsnce Score
        //performsnce Score = ((5 * GPU clock Speed) +(Number of Cores * CPU clock speed)) * multiplier

        int Perf_Score;

        Perf_Score = ((5 * clkspCPU)+(numCores * clkspCPU))*multiplier ;

        cout << "GPU Clock Speed: " ;
        <<clkspGPU<<endl ;
        cout << "CPU Clock Speed: " ;
        <<clkspCPU<<endl ;
        cout << "Number of cores: " ;
        <<numCores << endl;

        string reso;

        if (choice==1)
        {
            reso = "1280 * 720" ;
        }
        else if (choice==2)
        {
            reso= "1920 * 1080" ;
        }
        else if (choice==3)
        {
            reso="2560 *1440" ;
        
        }
        else if (choice==4)
        {
            reso="3840 * 2160" ;
        }
        else
        {
            cout <<"Error in entery\n" ;
        }
        cout << " Monitor Resolution: "
        <<reso<<endl;
        cout << "performsnce Score: "
        <<Perf_Score<<endl;

        if (Perf_Score > 17000)
        {
            cout << " Recommended Graphics Quality: Ultra\n\n" ;
        }
        else if (Perf_Score >=15000 && Perf_Score <=17000)
        {
            cout << " Recommended Graphics Quality: High\n\n" ;
        }
        else if (Perf_Score >=13000 && Perf_Score <=15000)
        {
            cout << " Recommended Graphics Quality: Medium\n\n" ;
        }
        else if (Perf_Score >=11000 && Perf_Score <=13000)
        {
            cout << " Recommended Graphics Quality: Low\n\n" ;
        }
        else 
        {
            cout << " Recommended Graphics Quality: Unable to play\n\n" ;
        }
        
        //Upadating the highest and lowest performsnce Variable

        if(Perf_Score > highPerf) highPerf = Perf_Score ;
        if (Perf_Score < lowPerf) lowPerf = Perf_Score ;




        numComputers--;

        //Displaying the highest and lowest performsnces score

        cout << endl;
        cout << "The highest performsnce score was: " << highPerf << endl ;
        cout << " The lowest performsnce score was: " << lowPerf << endl ;

        

    }
    retuern 0 ;
}
