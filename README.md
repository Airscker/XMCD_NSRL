# Manual of XMCDDP
## Download
Just Click [Here](https://minhaskamal.github.io/DownGit/#/home?url=https://github.com/Airscker/XMCD_NSRL/blob/main/XMCDDP.opx)
## Installation
- Just drag and drop the `.opx` file into Origin(need Origin 8.0 and upper editions) and we can find it in the list of APP (XMCDDP as below)

![alt Installation](https://github.com/Airscker/XMCD_NSRL/blob/main/img/app.jpg?raw=true)
## Usage
Open a dataset book and just click the app button, input the parameters we want to set and we will get results in the dataset book.

### 1.Open dataset book;
![alt book](https://github.com/Airscker/XMCD_NSRL/blob/main/img/book.jpg?raw=true)
### 2.Click app button and a small button will appear:
![alt app](https://github.com/Airscker/XMCD_NSRL/blob/main/img/click.jpg?raw=true)

Button is here:

![alt button](https://github.com/Airscker/XMCD_NSRL/blob/main/img/button.jpg?raw=true)
### 3.Input parameters and click OK
![alt parameters](https://github.com/Airscker/XMCD_NSRL/blob/main/img/sample.jpg?raw=true)
### 4.Get results
![alt results](https://github.com/Airscker/XMCD_NSRL/blob/main/img/res.jpg?raw=true)

## More Information
- Args:
	- `Start Value`:
	Where the x starts from, 760 defaultly
	
	- `End Value`
	Where the x ends, 810 defaultly
	
	- `Interpolated points`:
	The points we interpolated into curve, pay attention that we always have four valleys between five fingers so we'd better add another 1, such as that we want `dx` between every point is 0.5 we need set I.P as (810-760)/0.5+1=101
	
	- `Shifted Value`: 
	  The value we move the X axis, plus means right and negative means left, however, some tips we need to know that we don't allow the absolute shift value is smaller than `dx`, so if we input a shift value smaller than `dx`, program will change it to `dx` automatically. So if you want to improve the shift precision you need to improve the `Interpolated points` firstly.
	  
	  ![alt parameters](https://github.com/Airscker/XMCD_NSRL/blob/main/img/sample.jpg?raw=true)

- Results
	- `Interpolate`
	We will get two results which are `Linear interpolated data` and `Spline interpolated data`:
	
	![alt interpolate](https://github.com/Airscker/XMCD_NSRL/blob/main/img/inter.jpg?raw=true)
	
	- `Shifted`
	We will get many shifted data as below:
	
	![alt interpolate](https://github.com/Airscker/XMCD_NSRL/blob/main/img/shift.jpg?raw=true)
	
	- `Plot`
		We need to plot the result manually, the sample results are here (Red lines are shifted curve):
		- `shift=-2.5`
		
		![alt -2.5](https://github.com/Airscker/XMCD_NSRL/blob/main/img/-2.5.jpg?raw=true)
		
		- `shift=2.5`
		
		![alt 2.5](https://github.com/Airscker/XMCD_NSRL/blob/main/img/2.5.jpg?raw=true)