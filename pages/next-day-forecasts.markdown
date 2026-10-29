---
layout: page
title: California Next-Day Gridded Forecasts
permalink: /california-forecasts/
---

Grid-based forecast is one of the two forecasts types used for CSEP experiments and supported by PyCSEP. For a specific forecasting period, a grid-based forecast is specified by providing the expected number of events (or rate) for each square bin in a pre-defined space-magnitude grid. In this way, grid-based forecasts can be formatted as tables with each row representing a space-magnitude bin and each column reporting informations about the bin location (e.g. space coordinates, magnitude, depth). Grid-forecasts for multiple forecasting periods are then formatted as multiple tables, one for each period.

Here, we provide access to 27 models for California that, within CSEP, produced daily grid-based forecasts (between 00:00:01 and 23:59:59) of events with magnitude above 3.95 (or 4.95 depending on the model) and depth below 30 km, covering the period from August 1, 2007 to August 30, 2018 for a total of over 50,000 forecasts. These seismicity models includes several ensemble models, non-parametric models, and different flavors of the well-established Epidemic-Type Aftershock Sequence (ETAS), and Short-Term Earthquake Probability (STEP) models.

All the grid-based forecasts provided here are formatted accordingly to the [PyCSEP default format](https://docs.cseptesting.org/concepts/forecasts.html). They are a collection of .dat files (one for each day covered by the model) where row represents space-magnitude bins and column contains all the information needed to identify the bin and the rate. More specifically the columns (in order) are lower longitude extreme, upper longitude extreme, lower latitude extreme, upper latitude extreme, lower depth extreme, upper depth extreme, lower magnitude extreme, upper magnitude extreme, rate, and a flag. A more detailed explanation can be found on the PyCSEP website. All the forecasts are based on the same space-magnitude grid which consists of 0.1° x 0.1° (lat x lon), 0.1 Mw units, and one bin for the depth going from 0 to 30km.

The forecasts are provided as a .hdf5 file storing a system of nested folders. The system of nested folders is structered in the following way: one folder per year, inside each year folder we have one folder per month, and inside each month folder we have the .dat file representing the forecasts for the days of the respective month and year. We provided a tutorial (link) on how to use the .hdf5 file in combination with PyCSEP to evaluate the forecasts against observed data. This comprehends testing the consistency of the forecasts with the observations and comparing forecasts from different models.

# Code and Tutorial

The code to evaluate the forecasts against observed data, and the tutorial showing how to use the code, can be found [here](https://github.com/Serra314/CSEP-Next-day-gridded-forecast-database-for-California-code-and-tutorial/tree/main).

List of Models

To download the model, the user can download the models of interest using the Download links in the table below, or visit the download page with all the models at the following [link](https://g-3a9041.a78b8.36fe.data.globus.org/csep/csep1/files/index.html). Specific information on each model can be found following the Description links in the table.

<table>
  <thead>
    <tr>
      <th>Model name</th>
      <th>Starting date</th>
      <th>End date</th>
      <th>Missing days</th>
      <th>Min magnitude</th>
      <th>File dimension</th>
      <th>Links</th>
    </tr>
  </thead>
  <tbody>
    {% for item in site.data.models %}
      <tr>
        <td><strong>{{ item.model_name }}</strong></td>
        <td>{{ item.starting_date }}</td>
        <td>{{ item.end_date }}</td>
        <td>{{ item.missing_days }}</td>
        <td>{{ item.min_magnitude }}</td>
        <td>{{ item.file_dimension }}</td>
        <td>
          {% for link in item.links %}
            <a href="{{ link.url }}" class="table-link">{{ link.text }}</a>{% unless forloop.last %}, {% endunless %}
          {% endfor %}
        </td>
      </tr>
    {% endfor %}
  </tbody>
</table>
