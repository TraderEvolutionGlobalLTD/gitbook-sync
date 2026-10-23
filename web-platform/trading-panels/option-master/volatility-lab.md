# Volatility lab

The Volatility Lab tab provides a graphical representation of implied volatility (IV) values for selected option contracts. It allows users to visualize the volatility "smile" for different option series, helping to analyze market volatility before starting to trade options and has the following view:

<figure><img src="../../../.gitbook/assets/image (1453).png" alt=""><figcaption></figcaption></figure>

### Volatility smile plotting

Once a series (or multiple series) is selected, the volatility smile is plotted on the chart based on the following principles:

* Y-Axis: Represents the IV% (calculated using the Black-Scholes model in the).
* X-Axis (Basis): The X-axis scale depends on the _Basis_ setting in the panel:
  * Strike price - displays the strike prices on the X-axis.
  * Delta - displays the delta values of the options. The delta values are rounded to the nearest multiple of 5. The range for the delta scale varies based on the selected side.

**Plotting Logic:**

* Calls & Puts - the implied volatility is calculated for:
  * Call Strikes OTM (above the current last price).
  * Put Strikes OTM (below the current last price).
  * For ATM (at-the-money) strikes, the arithmetic mean of Call and Put strike IVs is used.
  * These data points are then combined into a single line on the chart.
* Calls or Puts - the implied volatility for all OTM Call or Put strikes is plotted on the Y-axis, and the values from the selected basis (Strike price or Delta) are plotted on the X-axis.

### Chart settings menu

The Settings panel is located to the right of the chart and allows users to control how the volatility smile is plotted. By default, the panel is open, but it can be collapsed by clicking the arrow next to the header.

1. Side - the drop-down list allows selecting an option side (strikes) on which the "Volatility lab" will be plotted. Available strikes are:
   * Calls & Puts (default);
   * Calls;
   * Puts.
2. Visible Series - a list of all available series based on the underlying asset selected in the lookup. Each series has:
   * A checkbox (unchecked by default) to select the series for plotting the volatility smile;
   * A color indicator to show the line color for the selected series. Note that the colors are predefined and can't be changed.

### Chart scaling

The chart view can be manipulated with the buttons![](https://help.za.velocitytrade.com/~gitbook/image?url=https%3A%2F%2F1243456536-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-legacy-files%2Fo%2Fassets%252F-LMCqxhh2XAdWPUjcvxR%252F-LNFbSGpWJc3pf9RFOCA%252F-LNFc1pNCZ83B6eNZf9U%252FScreenshot_5.png%3Falt%3Dmedia%26token%3Df0993924-e16c-49b1-b10e-5dcae11b6a3a\&width=300\&dpr=4\&quality=100\&sign=4965d795\&sv=1), located in the buttom-right corner of the chart field:

* Pressing the button![](https://help.za.velocitytrade.com/~gitbook/image?url=https%3A%2F%2F1243456536-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-legacy-files%2Fo%2Fassets%252F-LMCqxhh2XAdWPUjcvxR%252F-LNFbSGpWJc3pf9RFOCA%252F-LNFc9oLylMwR8qthi4F%252FScreenshot_12.png%3Falt%3Dmedia%26token%3Db284cc25-f172-4a17-9b33-a5ab948c3ad7\&width=300\&dpr=4\&quality=100\&sign=eb993b87\&sv=1)allows to zoom out of any random area of the chart;
* Pressing the button![](https://help.za.velocitytrade.com/~gitbook/image?url=https%3A%2F%2F1243456536-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-legacy-files%2Fo%2Fassets%252F-LMCqxhh2XAdWPUjcvxR%252F-LNFbSGpWJc3pf9RFOCA%252F-LNFcFSr_mpIPuvv0wwo%252FScreenshot_7.png%3Falt%3Dmedia%26token%3D9b4ef291-261e-4618-b2bb-efe910482d7a\&width=300\&dpr=4\&quality=100\&sign=c3176750\&sv=1)allows to zoom in to any random area of the chart;

The chart view can be also manipulated with some additional options:

* Hovering the cursor over a chart’s dot + mouse wheel scrolling - allows zooming in to and zooming out of a chosen dot![](https://help.za.velocitytrade.com/~gitbook/image?url=https%3A%2F%2F1243456536-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-legacy-files%2Fo%2Fassets%252F-LMCqxhh2XAdWPUjcvxR%252F-LNFcWXJLxz7jrWMbnO3%252F-LNFcja56QyaAG2TN7XX%252Fdd.png%3Falt%3Dmedia%26token%3D85141bd1-92d6-4a39-8465-7226d7fc748b\&width=300\&dpr=4\&quality=100\&sign=2b1b67e\&sv=1)of any chart;
* Clicking + holding + moving the cursor on a random area of the coordinate plane![](https://help.za.velocitytrade.com/~gitbook/image?url=https%3A%2F%2F1243456536-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-legacy-files%2Fo%2Fassets%252F-LMCqxhh2XAdWPUjcvxR%252F-LNFcWXJLxz7jrWMbnO3%252F-LNFcuURqZsW7vYtAk-N%252FScreenshot_14.png%3Falt%3Dmedia%26token%3D45098088-f7d7-4a59-81ee-3cefafd21bc3\&width=300\&dpr=4\&quality=100\&sign=912427fe\&sv=1)- allows to focus the chart view on this area of the coordinate plane;
* Clicking + moving the cursor on any area on the X or Y axis - allows to move on the left/right (X) or up/down (Y) on this area on the X or Y axis;
* Clicking + scrolling on any area on the X or Y axis - allows to zoom in to and zoom out of this area.
