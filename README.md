# Stream-Process-Manager
v. 2017.04.07

Design & code by Dr. Jordi Weiss.

Based on the "Operations Management" course by Prof. Suzanne de Treville at the University of Lausanne around 2015 to 2022.

The Stream Process Manager is a simulation-game I developed at the University of Lausanne with Prof. Suzanne de Treville to illustrate the process management aspects of the course.

--------------------------------------------------
## BASIC GUIDE

### Goal:

Your goal in this game is to maximize cash. To achieve this you will need to balance your production chain and your storage policy. Optimize your costs and your try to make your production fit with the demand.
Stocking materials or finished goods is costly, but stocking out leads to missing sales opportunities.


### Process:

The chronological steps of the production process are represented from the left to the right.
-	You first receive Raw Material, which is stored in the first warehouse (Raw Material Stock).

-	Then comes the Cutting stage. Raw material is taken from the Raw Material Stock and is processed by the workers and machines.

-	When a lot (depends on the lot size) is completed at the Cutting stage, it is stored in the intermediate warehouse (Intermediate Stock).

-	Then comes the Welding stage. Cut material is taken from the Intermediate Stock and is processed by the workers and machines.

-	When a lot (depends on the lot size) is completed at the Welding stage, it is stored in the final warehouse (Storage).

-	The finished products are sold depending on the demand.




### Indicators:

The indicators/output that you will need to check in order to take good decisions are displayed in the blue boxes. The overall results are displayed in the yellow box on the right.
Under each of the three warehouses (Raw Material Stock blue, Intermediate Stock and Storage), the blue box shows you the stock quantity and its cost. The warehouses icons can help you see quickly how your stock level throughout the production chain is. Each orange block represents 20 units, and the blocks become red when the stock is over 200. 

Under Cutting / Welding you can see:

-	The Capacity. Amount of pieces you can cut/weld during a cycle), which depends on the number of Workers and Machines you have. You can determine whether the bottleneck is the number of workers or of machines thanks to the utilization rate. 

-	The number of Scrapped pieces.

-	The Setup loss, number of pieces not produced due to Setup time, but not lost, unlike Scrap.

-	The Production.

-	The advancement of the Lot. The production at each cycle is added, until the lot is complete and sent to the next warehouse.

The costs depend on the number of workers and machines (3/cycle per worker, and 5/cycle per machine). 


The yellow box gives you the current Demand and the Sales, which are the minimum between the demand and what you have in final Storage. At each cycle, the “Costs” is the sum all of costs (Order, the 3 Warehouses, Cutting and Welding). Finally the Cash is just your previous cash + your sales – your costs of the period. 

**Information about demand**

-	Expected demand	216

-	Median demand	198

### User actions:

The user’s actions and input can be performed through the red boxes.
Under the Raw Material Order, you can manage the order quantity, for example on the picture above, the Raw Material warehouse seems to be overloaded (it is red with more than 300 units!), so it could be a good idea to reduce the order (which is now 45, as shown in the blue box), to a smaller number.
Under Cutting and Welding, you can manage your number of Worker and Machines, increase it or decrease it by one. Having more workers / machines will increase your capacity, but also your costs.
The bottom red rectangle allows you to apply policies globally to the whole chain.
The first option is a strict Quality Policy, reducing the scrap to 0, which has a unique cost of 5000.
The second option is the Setup Reduction. At a unique cost of 3000, it increases production at each cycle.
You can also manage lot size. Decreasing it allows quicker lot completion, making your production chain more fluid.

