### History

@ul
- You will be amazed
- What you can achieve
- *With a little imagination...*
- And **GitPitch Markdown**
@ulend

---

### History 2

- You will be amazed
- What you can achieve
- *With a little imagination...*
- And **GitPitch Markdown**


---

### Code

  SLV.Control.MeaningsHistoryChartsContainer.prototype._addHistoryChart = function (device) {
    var chart = this.charts.filter(function (c) { return c.device === device; });
    if (!chart || chart.length == 0) {
        chart = new SLV.Control.MeaningsHistoryChart(this, device);
        chart.target.style.top = (this.charts.length * (SLV.Control.MeaningsHistoryChart.CHART_HEIGHT + SLV.Control.MeaningsHistoryChart.CHART_TITLE_HEIGHT)) + 'px';
        this.chartsContainer.appendChild(chart.target);
        this.charts.push(chart);
        chart.initialize();
        this._syncCursorWithOtherCharts(chart);
        return chart;
    }
    else {
        return chart[0];
    }
};
