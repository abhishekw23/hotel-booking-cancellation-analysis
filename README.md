 Project Overview
Analysis of hotel booking data to identify cancellation patterns, seasonal pricing trends, and Average Daily Rate (ADR) behavior across City Hotels and Resort Hotels. This project helps understand what drives hotel booking cancellations.

 Objective

Find the overall cancellation rate for hotel bookings
Compare cancellations between City Hotel and Resort Hotel
Analyze Average Daily Rate (ADR) trends over time
Identify which months have the highest cancellations
Find Top 10 countries with the most cancellations
Study the market segment (Online TA, Direct, Corporate, etc.) distribution
Compare ADR for cancelled vs non-cancelled bookings


 Dataset
DetailInfoFilehotel_booking.csvKey Columnshotel, is_canceled, adr, reservation_status_date, country, market_segment

 Tools & Libraries
ToolPurposePythonCore programmingPandasData loading, cleaning, manipulationMatplotlibLine charts, bar charts, pie chartsSeabornCount plots for categorical comparisons

 Data Cleaning Steps

Converted reservation_status_date to datetime format
Dropped company and agent columns (too many missing values)
Removed remaining null rows using dropna()
Filtered out extreme ADR values above 5000 (outlier removal)


 Visualizations
ChartDescriptionBar ChartOverall cancellation percentageCount PlotCancellations by hotel type (City vs Resort)Line ChartAverage Daily Rate over time for both hotel typesCount PlotMonthly reservation status (cancelled vs not cancelled)Bar ChartTotal ADR per month for cancelled bookingsPie ChartTop 10 countries with most cancellationsLine ChartADR comparison between cancelled and non-cancelled bookings

 Key Insights

Around 37% of total bookings were cancelled
City Hotels have a higher cancellation rate than Resort Hotels
Resort Hotels charge higher ADR during peak seasons
Cancellations peak in July and August (summer months)
Portugal (PRT) accounts for the highest share of cancellations
Online Travel Agents (OTA) dominate the market segment
Higher ADR is observed in cancelled bookings compared to non-cancelled ones


 Project Structure
hotel-booking-cancellation-analysis/
│
├── Hotel_Booking.ipynb     # Main analysis notebook
├── hotel_booking.csv       # Dataset
├── README.md               # Project documentation

 How to Run

Clone this repository
Install required libraries:

bash   pip install pandas matplotlib seaborn

Open Hotel_Booking.ipynb in Jupyter Notebook or VS Code
Run all cells
