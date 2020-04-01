# COVID19

Topic: Modelling the exponential growth of the COVID19 cases in Switzerland.

Numerous reports focus on the development of case numbers over time. But hardly anyone talks about the growth and whether the measures we are taking in the fight against COVID19 are having an effect, in other words: are we beating the virus?

In mathematical epidemiology, time has no influence on the development of case numbers. In the SIR model, the three decisive variables are: Susceptible, Infected, Removed.

Therefore, in my presentation of the case numbers I will show new cases ~ Total confirmed cases. This is a better way to graph cases using a logarithmic scale in “phase space” - plotting the growth rate against the cumulative cases, rather than either of these against time. In this way it can be seen whether the growth is slowing down, i.e. whether the case numbers are no longer developing exponentially.

Inspiration for this presentation comes from this video by minutephysics (https://www.youtube.com/watch?v=54XLXg4fYsc) and the underlying dashboard build by Aatish Bhatia (https://github.com/aatishb/covid/blob/master/curvefit.ipynb).

Here’s Ben Spark explaining the SIR model in a wonderfully simple and understandable manner: https://www.youtube.com/watch?v=k6nLfCbAzgo
Variables:

    Date: Date cases were reported
    Cases: Number of people tested positive on that date
    Total_Cases: Cumulative count of cases as of that date
    New_Cases: Number of cases compared to the previous date
    Week: Grouping dates to calendar weeks according to ISO8601

Source: Bundesamt für Gesundheit (BAG), Daten des Situationsberichtes, Last retrieved: 31.03.2020
