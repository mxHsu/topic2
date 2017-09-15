#include <iostream>
#include <opencv2/core/core.hpp>
#include <opencv2/highgui/highgui.hpp>
#include <opencv2/opencv.hpp>

using namespace cv;
using namespace std;

int main( )
{
    Mat image=imread("/Users/macbookair/Desktop/timg.jpg");
    if(image.empty())
    {
        cout<<"Error!cannot be read...../n";
        return -1;
    }
    namedWindow("original image");
    imshow("original image", image);
    waitKey(0);
    
}
