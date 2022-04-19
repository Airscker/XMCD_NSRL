# Manual of XMCDDP
## Installation
- Just drag and drop the `.opx` file into Origin(need Origin 8.0 and upper editions) and we can find it in the list of APP

## Usage
- Args:
	`Start Value`:
	Where the x starts from, 760 defaultly
	`End Value`
	Where the x ends, 810 defaultly
	`Interpolated points`:
	The points we interpolated into curve, pay attention that we always have four valleys between five fingers so we'd better add another 1, such as that we want `dx` between every point is 0.5 we need set I.P as (810-760)/0.5+1=101
	`Shifted Value`: 
	The value we move the X axis, plus means right and negative means left, however, some tips we need to know that we don't allow the absolute shift value is smaller than `dx`, so if we input a shift value smaller than `dx`, program will change it to `dx` automatically. So if you want to improve the shift precision you need to improve the `Interpolated points` firstly.
- Operation
	`Interpolate`
	We will get two results which are `Linear interpolated data` and `Spline interpolated data`