# Progress

## 7/10/2020

Today we began planing out the tools we will use to create the dashboard. A Glitter chat was setup and planned to meet on video every Monday at 1pm. We plan to setup the tools to access the data we will be working with as well as the jupyter notebook we will be using to construct everything.

## 7/17/2020

The project is slowly moving along. We have successfully added a visual representation of the COG data. The option to toggle through diffrent places was also added so that the user will be able choose what data they want to look at. The programmer has to put them in manualy though. Currently working on having the dashboard display the maximum and minimum heights of the data set. Soon we will have to look into having the program somehow let the user select from the data which is in the cloud.

## 7/24/2020

A lot of progress was made this week. Essentially all we have worked on was put together as one. The functions from **xarray-spatial** were added. A user can select between using **shade, quantile, slope and aspect**. A special slider has been added which allows for choosing a range of values which you would like to examine (for example all parts of the map whose height is between 40 and 200 meters). For the quantile function you can select how many levels you want to use. Unfortunalty, the curvature is presenting some problems but that will be sorted out. The user can also select the **color map** that they want to use as well.

## 7/31/2020

After consulting an Anaconda Programmer, we learned that we had to resturcture the program. The the initial version consisted of one very large function which created all the displays. The program has now been reformated so that each individual option is seperated into **tabs** which have their own isolated display (curvature is now avaliable as well). There is now an options tab to select the color map. The options tab now also includes an **interactive map on which you can select what location you want to see in the US by clicking** instead of the preset locations before. The program automatically pulls the required data from the Amazon Bucket. Now moving forward we must add more xarray functions as well as deal with some noticable prefomance errors.  

## 8/7/2020

This week was a bit slower. We are in the process of allowing the user to select a region smaller than a 1 degree region, as well as fixing issues with the slope,and curvature functions. For these issues we are consulting knowledgebale people on how to fix them so it is taking a little bit. By Monday a temporary region selector will be in place.

## 8/14/2020

This week was spent working out problems with the slope and curvature functions and developing a way to allow selecting smaller than one degree squares. After asking on Stack Overflow and the Xarray github, we figured out how merge different data sets in xarray. In addition, we learned after speaking with an xarray spatial developer how to fix the issues we were having with curvature and slope by changing the resolution. Currently these new features are being added to the dashboard. Next week as we move to the end of the project we may look into slecting different overviews.
