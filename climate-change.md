# Climate Change Portfolio Post

Climate change is impacting the way people live around the world. Higher highs, lower lows, storms, and smoke – we’re all feeling the
effects of climate change. Here, we look at trends in temperature over time along the San Pedro River in Arizona.

## Wrangle data

### Load Python packages


<script type="esms-options">{"shimMode": true}</script><style>*[data-root-id],
*[data-root-id] > * {
  box-sizing: border-box;
  font-family: var(--jp-ui-font-family);
  font-size: var(--jp-ui-font-size1);
  color: var(--vscode-editor-foreground, var(--jp-ui-font-color1));
}

/* Override VSCode background color */
.cell-output-ipywidget-background:has(
  > .cell-output-ipywidget-background > .lm-Widget > *[data-root-id]
),
.cell-output-ipywidget-background:has(> .lm-Widget > *[data-root-id]) {
  background-color: transparent !important;
}
</style>







<div id='p1189'>
  <div id="e2be4c5e-33dd-4002-ba33-9ad7b23a67c1" data-root-id="p1189" style="display: contents;"></div>
</div>
<script type="application/javascript">(function(root) {
  var docs_json = {"f012e3ab-0416-44dc-a754-30b76c45d33e":{"version":"3.8.0","title":"Bokeh Application","config":{"type":"object","name":"DocumentConfig","id":"p1187","attributes":{"notifications":{"type":"object","name":"Notifications","id":"p1188"}}},"roots":[{"type":"object","name":"panel.models.browser.BrowserInfo","id":"p1189"},{"type":"object","name":"panel.models.comm_manager.CommManager","id":"p1190","attributes":{"plot_id":"p1189","comm_id":"749c14623e1a4eed858a13d9a7afa71c","client_comm_id":"d00f5f9a949f401e85365ab65162bc1d"}}],"defs":[{"type":"model","name":"ReactiveHTML1"},{"type":"model","name":"FlexBox1","properties":[{"name":"align_content","kind":"Any","default":"flex-start"},{"name":"align_items","kind":"Any","default":"flex-start"},{"name":"flex_direction","kind":"Any","default":"row"},{"name":"flex_wrap","kind":"Any","default":"wrap"},{"name":"gap","kind":"Any","default":""},{"name":"justify_content","kind":"Any","default":"flex-start"}]},{"type":"model","name":"FloatPanel1","properties":[{"name":"config","kind":"Any","default":{"type":"map"}},{"name":"contained","kind":"Any","default":true},{"name":"position","kind":"Any","default":"right-top"},{"name":"offsetx","kind":"Any","default":null},{"name":"offsety","kind":"Any","default":null},{"name":"theme","kind":"Any","default":"primary"},{"name":"status","kind":"Any","default":"normalized"}]},{"type":"model","name":"GridStack1","properties":[{"name":"ncols","kind":"Any","default":null},{"name":"nrows","kind":"Any","default":null},{"name":"allow_resize","kind":"Any","default":true},{"name":"allow_drag","kind":"Any","default":true},{"name":"state","kind":"Any","default":[]}]},{"type":"model","name":"drag1","properties":[{"name":"slider_width","kind":"Any","default":5},{"name":"slider_color","kind":"Any","default":"black"},{"name":"start","kind":"Any","default":0},{"name":"end","kind":"Any","default":100},{"name":"value","kind":"Any","default":50}]},{"type":"model","name":"click1","properties":[{"name":"terminal_output","kind":"Any","default":""},{"name":"debug_name","kind":"Any","default":""},{"name":"clears","kind":"Any","default":0}]},{"type":"model","name":"ReactiveESM1","properties":[{"name":"esm_constants","kind":"Any","default":{"type":"map"}}]},{"type":"model","name":"JSComponent1","properties":[{"name":"esm_constants","kind":"Any","default":{"type":"map"}}]},{"type":"model","name":"ReactComponent1","properties":[{"name":"use_shadow_dom","kind":"Any","default":true},{"name":"esm_constants","kind":"Any","default":{"type":"map"}}]},{"type":"model","name":"AnyWidgetComponent1","properties":[{"name":"use_shadow_dom","kind":"Any","default":true},{"name":"esm_constants","kind":"Any","default":{"type":"map"}}]},{"type":"model","name":"FastWrapper1","properties":[{"name":"object","kind":"Any","default":null},{"name":"style","kind":"Any","default":null}]},{"type":"model","name":"NotificationArea1","properties":[{"name":"js_events","kind":"Any","default":{"type":"map"}},{"name":"max_notifications","kind":"Any","default":5},{"name":"notifications","kind":"Any","default":[]},{"name":"position","kind":"Any","default":"bottom-right"},{"name":"_clear","kind":"Any","default":0},{"name":"types","kind":"Any","default":[{"type":"map","entries":[["type","warning"],["background","#ffc107"],["icon",{"type":"map","entries":[["className","fas fa-exclamation-triangle"],["tagName","i"],["color","white"]]}]]},{"type":"map","entries":[["type","info"],["background","#007bff"],["icon",{"type":"map","entries":[["className","fas fa-info-circle"],["tagName","i"],["color","white"]]}]]}]}]},{"type":"model","name":"Notification","properties":[{"name":"background","kind":"Any","default":null},{"name":"duration","kind":"Any","default":3000},{"name":"icon","kind":"Any","default":null},{"name":"message","kind":"Any","default":""},{"name":"notification_type","kind":"Any","default":null},{"name":"_rendered","kind":"Any","default":false},{"name":"_destroyed","kind":"Any","default":false}]},{"type":"model","name":"TemplateActions1","properties":[{"name":"open_modal","kind":"Any","default":0},{"name":"close_modal","kind":"Any","default":0}]},{"type":"model","name":"BootstrapTemplateActions1","properties":[{"name":"open_modal","kind":"Any","default":0},{"name":"close_modal","kind":"Any","default":0}]},{"type":"model","name":"TemplateEditor1","properties":[{"name":"layout","kind":"Any","default":[]}]},{"type":"model","name":"MaterialTemplateActions1","properties":[{"name":"open_modal","kind":"Any","default":0},{"name":"close_modal","kind":"Any","default":0}]},{"type":"model","name":"request_value1","properties":[{"name":"fill","kind":"Any","default":"none"},{"name":"_synced","kind":"Any","default":null},{"name":"_request_sync","kind":"Any","default":0}]}]}};
  var render_items = [{"docid":"f012e3ab-0416-44dc-a754-30b76c45d33e","roots":{"p1189":"e2be4c5e-33dd-4002-ba33-9ad7b23a67c1"},"root_ids":["p1189"]}];
  var docs = Object.values(docs_json)
  if (!docs) {
    return
  }
  const py_version = docs[0].version.replace('rc', '-rc.').replace('.dev', '-dev.')
  async function embed_document(root) {
    var Bokeh = get_bokeh(root)
    await Bokeh.embed.embed_items_notebook(docs_json, render_items);
    for (const render_item of render_items) {
      for (const root_id of render_item.root_ids) {
	const id_el = document.getElementById(root_id)
	if (id_el.children.length && id_el.children[0].hasAttribute('data-root-id')) {
	  const root_el = id_el.children[0]
	  root_el.id = root_el.id + '-rendered'
	  for (const child of root_el.children) {
            // Ensure JupyterLab does not capture keyboard shortcuts
            // see: https://jupyterlab.readthedocs.io/en/4.1.x/extension/notebook.html#keyboard-interaction-model
	    child.setAttribute('data-lm-suppress-shortcuts', 'true')
	  }
	}
      }
    }
  }
  function get_bokeh(root) {
    if (root.Bokeh === undefined) {
      return null
    } else if (root.Bokeh.version !== py_version) {
      if (root.Bokeh.versions === undefined || !root.Bokeh.versions.has(py_version)) {
	return null
      }
      return root.Bokeh.versions.get(py_version);
    } else if (root.Bokeh.version === py_version) {
      return root.Bokeh
    }
    return null
  }
  function is_loaded(root) {
    var Bokeh = get_bokeh(root)
    return (Bokeh != null && Bokeh.Panel !== undefined)
  }
  if (is_loaded(root)) {
    embed_document(root);
  } else {
    var attempts = 0;
    var timer = setInterval(function(root) {
      if (is_loaded(root)) {
        clearInterval(timer);
        embed_document(root);
      } else if (document.readyState == "complete") {
        attempts++;
        if (attempts > 200) {
          clearInterval(timer);
	  var Bokeh = get_bokeh(root)
	  if (Bokeh == null || Bokeh.Panel == null) {
            console.warn("Panel: ERROR: Unable to run Panel code because Bokeh or Panel library is missing");
	  } else {
	    console.warn("Panel: WARNING: Attempting to render but not all required libraries could be resolved.")
	    embed_document(root)
	  }
        }
      }
    }, 25, root)
  }
})(window);</script>


### Download the data

I've downloaded some climate data from NCEI for the Muleshoe Ranch Station in Southeast Arizona in CSV format (https://www.ncei.noaa.gov/cdo-web/datasets/GHCND/stations/GHCND:USR0000AMUL/detail). I'm interested in this area because some of my research focuses on assessing floodplain organic carbon stocks along the San Pedro River, AZ, which this station is located right next to. 

Southeast Arizona has an arid climate and has been experiencing an extended drought. I'm interested in seeing whether there is a significant trend in temperature over the last few decades in this region near one of my study sites.

In the field, we saw that many riparian areas that were altered by human activities had depleted ground water levels, reduced presence of large native vegetation, and in some places, the channel had completely dried up. I would hypothesize that increased mean annual temperatures may have exacerbated some of these changes that we observed.




    pandas.core.frame.DataFrame



### Clean up the `DataFrame`




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>TAVG</th>
    </tr>
    <tr>
      <th>DATE</th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>1988-04-05</th>
      <td>70</td>
    </tr>
    <tr>
      <th>1988-04-06</th>
      <td>67</td>
    </tr>
    <tr>
      <th>1988-04-28</th>
      <td>59</td>
    </tr>
    <tr>
      <th>1988-04-29</th>
      <td>60</td>
    </tr>
    <tr>
      <th>1988-04-30</th>
      <td>69</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
    </tr>
    <tr>
      <th>2026-09-13</th>
      <td>77</td>
    </tr>
    <tr>
      <th>2026-09-14</th>
      <td>76</td>
    </tr>
    <tr>
      <th>2026-09-15</th>
      <td>75</td>
    </tr>
    <tr>
      <th>2026-09-16</th>
      <td>70</td>
    </tr>
    <tr>
      <th>2026-09-17</th>
      <td>74</td>
    </tr>
  </tbody>
</table>
<p>14000 rows × 1 columns</p>
</div>



### Convert the units

Here we'll make sure we're using the right units by converting from F to C.

We'll do this by creating a function for the unit conversion.

## Plot the temperature data

Here we'll plot all of the daily temperature data. This will show us whether there are any gaps in the data or any measurements that look incorrect. 


    
![png](climate-change_files/climate-change_13_0.png)
    


### Clean up time series plots by resampling

Now we'll resample the data. This summarizes the data as an annual mean value, giving us one data point per year.




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>temp_f</th>
      <th>temp_c</th>
    </tr>
    <tr>
      <th>DATE</th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>1988-01-01</th>
      <td>69.481781</td>
      <td>20.823212</td>
    </tr>
    <tr>
      <th>1989-01-01</th>
      <td>64.482192</td>
      <td>18.045662</td>
    </tr>
    <tr>
      <th>1990-01-01</th>
      <td>61.824658</td>
      <td>16.569254</td>
    </tr>
    <tr>
      <th>1991-01-01</th>
      <td>61.413699</td>
      <td>16.340944</td>
    </tr>
    <tr>
      <th>1992-01-01</th>
      <td>61.816940</td>
      <td>16.564967</td>
    </tr>
    <tr>
      <th>1993-01-01</th>
      <td>63.158192</td>
      <td>17.310107</td>
    </tr>
    <tr>
      <th>1994-01-01</th>
      <td>63.623626</td>
      <td>17.568681</td>
    </tr>
    <tr>
      <th>1995-01-01</th>
      <td>63.522099</td>
      <td>17.512277</td>
    </tr>
    <tr>
      <th>1996-01-01</th>
      <td>64.123288</td>
      <td>17.846271</td>
    </tr>
    <tr>
      <th>1997-01-01</th>
      <td>63.024793</td>
      <td>17.235996</td>
    </tr>
    <tr>
      <th>1998-01-01</th>
      <td>61.865753</td>
      <td>16.592085</td>
    </tr>
    <tr>
      <th>1999-01-01</th>
      <td>63.734247</td>
      <td>17.630137</td>
    </tr>
    <tr>
      <th>2000-01-01</th>
      <td>64.469945</td>
      <td>18.038859</td>
    </tr>
    <tr>
      <th>2001-01-01</th>
      <td>62.830137</td>
      <td>17.127854</td>
    </tr>
    <tr>
      <th>2002-01-01</th>
      <td>64.306849</td>
      <td>17.948250</td>
    </tr>
    <tr>
      <th>2003-01-01</th>
      <td>64.528767</td>
      <td>18.071537</td>
    </tr>
    <tr>
      <th>2004-01-01</th>
      <td>63.166667</td>
      <td>17.314815</td>
    </tr>
    <tr>
      <th>2005-01-01</th>
      <td>64.227397</td>
      <td>17.904110</td>
    </tr>
    <tr>
      <th>2006-01-01</th>
      <td>63.767123</td>
      <td>17.648402</td>
    </tr>
    <tr>
      <th>2007-01-01</th>
      <td>64.002740</td>
      <td>17.779300</td>
    </tr>
    <tr>
      <th>2008-01-01</th>
      <td>63.319672</td>
      <td>17.399818</td>
    </tr>
    <tr>
      <th>2009-01-01</th>
      <td>64.882192</td>
      <td>18.267884</td>
    </tr>
    <tr>
      <th>2010-01-01</th>
      <td>63.298630</td>
      <td>17.388128</td>
    </tr>
    <tr>
      <th>2011-01-01</th>
      <td>63.802740</td>
      <td>17.668189</td>
    </tr>
    <tr>
      <th>2012-01-01</th>
      <td>64.885246</td>
      <td>18.269581</td>
    </tr>
    <tr>
      <th>2013-01-01</th>
      <td>63.635616</td>
      <td>17.575342</td>
    </tr>
    <tr>
      <th>2014-01-01</th>
      <td>64.947945</td>
      <td>18.304414</td>
    </tr>
    <tr>
      <th>2015-01-01</th>
      <td>63.813699</td>
      <td>17.674277</td>
    </tr>
    <tr>
      <th>2016-01-01</th>
      <td>64.587912</td>
      <td>18.104396</td>
    </tr>
    <tr>
      <th>2017-01-01</th>
      <td>65.950685</td>
      <td>18.861492</td>
    </tr>
    <tr>
      <th>2018-01-01</th>
      <td>64.402740</td>
      <td>18.001522</td>
    </tr>
    <tr>
      <th>2019-01-01</th>
      <td>62.879452</td>
      <td>17.155251</td>
    </tr>
    <tr>
      <th>2020-01-01</th>
      <td>65.461749</td>
      <td>18.589860</td>
    </tr>
    <tr>
      <th>2021-01-01</th>
      <td>64.586301</td>
      <td>18.103501</td>
    </tr>
    <tr>
      <th>2022-01-01</th>
      <td>63.446575</td>
      <td>17.470320</td>
    </tr>
    <tr>
      <th>2023-01-01</th>
      <td>64.934066</td>
      <td>18.296703</td>
    </tr>
    <tr>
      <th>2024-01-01</th>
      <td>64.986339</td>
      <td>18.325744</td>
    </tr>
    <tr>
      <th>2025-01-01</th>
      <td>66.153425</td>
      <td>18.974125</td>
    </tr>
    <tr>
      <th>2026-01-01</th>
      <td>70.061538</td>
      <td>21.145299</td>
    </tr>
  </tbody>
</table>
</div>



## Plot the annual data




    <Axes: title={'center': 'Mean Annual Temperature in Arizona'}, xlabel='Year', ylabel='Temperature ($^\\circ$C)'>




    
![png](climate-change_files/climate-change_17_1.png)
    


>**Plot Interpretations**
>* We see that in the first and last year of data, the plotted mean annual temperature is extremely high compared to other years. This is caused by incomplete data. 2026 isn't over yet, and data from 1988 starts in April, so it would be a good idea to remove these years.
>* Mean annual temperatures are lower in the 1990s than they are in the 2020s. While this isn't a particularly long study period, this trend in 35+ years of data could be a result of climate change. It is difficult to say that conclusively without further analysis/looking at the data more closely.

## Make an interactive plot


<script type="esms-options">{"shimMode": true}</script><style>*[data-root-id],
*[data-root-id] > * {
  box-sizing: border-box;
  font-family: var(--jp-ui-font-family);
  font-size: var(--jp-ui-font-size1);
  color: var(--vscode-editor-foreground, var(--jp-ui-font-color1));
}

/* Override VSCode background color */
.cell-output-ipywidget-background:has(
  > .cell-output-ipywidget-background > .lm-Widget > *[data-root-id]
),
.cell-output-ipywidget-background:has(> .lm-Widget > *[data-root-id]) {
  background-color: transparent !important;
}
</style>







<div id='p1193'>
  <div id="c31c7701-ff0c-4f6d-adbf-43aa216d0444" data-root-id="p1193" style="display: contents;"></div>
</div>
<script type="application/javascript">(function(root) {
  var docs_json = {"4ec5750f-d8e8-4fe6-ad34-b398b886cb93":{"version":"3.8.0","title":"Bokeh Application","config":{"type":"object","name":"DocumentConfig","id":"p1191","attributes":{"notifications":{"type":"object","name":"Notifications","id":"p1192"}}},"roots":[{"type":"object","name":"panel.models.browser.BrowserInfo","id":"p1193"},{"type":"object","name":"panel.models.comm_manager.CommManager","id":"p1194","attributes":{"plot_id":"p1193","comm_id":"4ff1110e25974d01997a8031fdc049ab","client_comm_id":"98268ef436654b498cd0a6cf9b09ce5e"}}],"defs":[{"type":"model","name":"ReactiveHTML1"},{"type":"model","name":"FlexBox1","properties":[{"name":"align_content","kind":"Any","default":"flex-start"},{"name":"align_items","kind":"Any","default":"flex-start"},{"name":"flex_direction","kind":"Any","default":"row"},{"name":"flex_wrap","kind":"Any","default":"wrap"},{"name":"gap","kind":"Any","default":""},{"name":"justify_content","kind":"Any","default":"flex-start"}]},{"type":"model","name":"FloatPanel1","properties":[{"name":"config","kind":"Any","default":{"type":"map"}},{"name":"contained","kind":"Any","default":true},{"name":"position","kind":"Any","default":"right-top"},{"name":"offsetx","kind":"Any","default":null},{"name":"offsety","kind":"Any","default":null},{"name":"theme","kind":"Any","default":"primary"},{"name":"status","kind":"Any","default":"normalized"}]},{"type":"model","name":"GridStack1","properties":[{"name":"ncols","kind":"Any","default":null},{"name":"nrows","kind":"Any","default":null},{"name":"allow_resize","kind":"Any","default":true},{"name":"allow_drag","kind":"Any","default":true},{"name":"state","kind":"Any","default":[]}]},{"type":"model","name":"drag1","properties":[{"name":"slider_width","kind":"Any","default":5},{"name":"slider_color","kind":"Any","default":"black"},{"name":"start","kind":"Any","default":0},{"name":"end","kind":"Any","default":100},{"name":"value","kind":"Any","default":50}]},{"type":"model","name":"click1","properties":[{"name":"terminal_output","kind":"Any","default":""},{"name":"debug_name","kind":"Any","default":""},{"name":"clears","kind":"Any","default":0}]},{"type":"model","name":"ReactiveESM1","properties":[{"name":"esm_constants","kind":"Any","default":{"type":"map"}}]},{"type":"model","name":"JSComponent1","properties":[{"name":"esm_constants","kind":"Any","default":{"type":"map"}}]},{"type":"model","name":"ReactComponent1","properties":[{"name":"use_shadow_dom","kind":"Any","default":true},{"name":"esm_constants","kind":"Any","default":{"type":"map"}}]},{"type":"model","name":"AnyWidgetComponent1","properties":[{"name":"use_shadow_dom","kind":"Any","default":true},{"name":"esm_constants","kind":"Any","default":{"type":"map"}}]},{"type":"model","name":"FastWrapper1","properties":[{"name":"object","kind":"Any","default":null},{"name":"style","kind":"Any","default":null}]},{"type":"model","name":"NotificationArea1","properties":[{"name":"js_events","kind":"Any","default":{"type":"map"}},{"name":"max_notifications","kind":"Any","default":5},{"name":"notifications","kind":"Any","default":[]},{"name":"position","kind":"Any","default":"bottom-right"},{"name":"_clear","kind":"Any","default":0},{"name":"types","kind":"Any","default":[{"type":"map","entries":[["type","warning"],["background","#ffc107"],["icon",{"type":"map","entries":[["className","fas fa-exclamation-triangle"],["tagName","i"],["color","white"]]}]]},{"type":"map","entries":[["type","info"],["background","#007bff"],["icon",{"type":"map","entries":[["className","fas fa-info-circle"],["tagName","i"],["color","white"]]}]]}]}]},{"type":"model","name":"Notification","properties":[{"name":"background","kind":"Any","default":null},{"name":"duration","kind":"Any","default":3000},{"name":"icon","kind":"Any","default":null},{"name":"message","kind":"Any","default":""},{"name":"notification_type","kind":"Any","default":null},{"name":"_rendered","kind":"Any","default":false},{"name":"_destroyed","kind":"Any","default":false}]},{"type":"model","name":"TemplateActions1","properties":[{"name":"open_modal","kind":"Any","default":0},{"name":"close_modal","kind":"Any","default":0}]},{"type":"model","name":"BootstrapTemplateActions1","properties":[{"name":"open_modal","kind":"Any","default":0},{"name":"close_modal","kind":"Any","default":0}]},{"type":"model","name":"TemplateEditor1","properties":[{"name":"layout","kind":"Any","default":[]}]},{"type":"model","name":"MaterialTemplateActions1","properties":[{"name":"open_modal","kind":"Any","default":0},{"name":"close_modal","kind":"Any","default":0}]},{"type":"model","name":"request_value1","properties":[{"name":"fill","kind":"Any","default":"none"},{"name":"_synced","kind":"Any","default":null},{"name":"_request_sync","kind":"Any","default":0}]}]}};
  var render_items = [{"docid":"4ec5750f-d8e8-4fe6-ad34-b398b886cb93","roots":{"p1193":"c31c7701-ff0c-4f6d-adbf-43aa216d0444"},"root_ids":["p1193"]}];
  var docs = Object.values(docs_json)
  if (!docs) {
    return
  }
  const py_version = docs[0].version.replace('rc', '-rc.').replace('.dev', '-dev.')
  async function embed_document(root) {
    var Bokeh = get_bokeh(root)
    await Bokeh.embed.embed_items_notebook(docs_json, render_items);
    for (const render_item of render_items) {
      for (const root_id of render_item.root_ids) {
	const id_el = document.getElementById(root_id)
	if (id_el.children.length && id_el.children[0].hasAttribute('data-root-id')) {
	  const root_el = id_el.children[0]
	  root_el.id = root_el.id + '-rendered'
	  for (const child of root_el.children) {
            // Ensure JupyterLab does not capture keyboard shortcuts
            // see: https://jupyterlab.readthedocs.io/en/4.1.x/extension/notebook.html#keyboard-interaction-model
	    child.setAttribute('data-lm-suppress-shortcuts', 'true')
	  }
	}
      }
    }
  }
  function get_bokeh(root) {
    if (root.Bokeh === undefined) {
      return null
    } else if (root.Bokeh.version !== py_version) {
      if (root.Bokeh.versions === undefined || !root.Bokeh.versions.has(py_version)) {
	return null
      }
      return root.Bokeh.versions.get(py_version);
    } else if (root.Bokeh.version === py_version) {
      return root.Bokeh
    }
    return null
  }
  function is_loaded(root) {
    var Bokeh = get_bokeh(root)
    return (Bokeh != null && Bokeh.Panel !== undefined)
  }
  if (is_loaded(root)) {
    embed_document(root);
  } else {
    var attempts = 0;
    var timer = setInterval(function(root) {
      if (is_loaded(root)) {
        clearInterval(timer);
        embed_document(root);
      } else if (document.readyState == "complete") {
        attempts++;
        if (attempts > 200) {
          clearInterval(timer);
	  var Bokeh = get_bokeh(root)
	  if (Bokeh == null || Bokeh.Panel == null) {
            console.warn("Panel: ERROR: Unable to run Panel code because Bokeh or Panel library is missing");
	  } else {
	    console.warn("Panel: WARNING: Attempting to render but not all required libraries could be resolved.")
	    embed_document(root)
	  }
        }
      }
    }, 25, root)
  }
})(window);</script>







<div id='p1197'>
  <div id="f634fe9b-0226-4fcd-b82c-19ca37ce56d1" data-root-id="p1197" style="display: contents;"></div>
</div>
<script type="application/javascript">(function(root) {
  var docs_json = {"9b2b1f88-4013-4700-9a09-132017edb0ce":{"version":"3.8.0","title":"Bokeh Application","config":{"type":"object","name":"DocumentConfig","id":"p1195","attributes":{"notifications":{"type":"object","name":"Notifications","id":"p1196"}}},"roots":[{"type":"object","name":"Row","id":"p1197","attributes":{"name":"Row01112","tags":["embedded"],"stylesheets":["\n:host(.pn-loading):before, .pn-loading:before {\n  background-color: #c3c3c3;\n  mask-size: auto calc(min(50%, 300px));\n  -webkit-mask-size: auto calc(min(50%, 300px));\n}",{"type":"object","name":"ImportedStyleSheet","id":"p1200","attributes":{"url":"https://cdn.holoviz.org/panel/1.8.0/dist/css/loading.css"}},{"type":"object","name":"ImportedStyleSheet","id":"p1272","attributes":{"url":"https://cdn.holoviz.org/panel/1.8.0/dist/css/listpanel.css"}},{"type":"object","name":"ImportedStyleSheet","id":"p1198","attributes":{"url":"https://cdn.holoviz.org/panel/1.8.0/dist/bundled/theme/default.css"}},{"type":"object","name":"ImportedStyleSheet","id":"p1199","attributes":{"url":"https://cdn.holoviz.org/panel/1.8.0/dist/bundled/theme/native.css"}}],"min_width":700,"margin":0,"sizing_mode":"stretch_width","align":"start","children":[{"type":"object","name":"Spacer","id":"p1201","attributes":{"name":"HSpacer01119","stylesheets":["\n:host(.pn-loading):before, .pn-loading:before {\n  background-color: #c3c3c3;\n  mask-size: auto calc(min(50%, 300px));\n  -webkit-mask-size: auto calc(min(50%, 300px));\n}",{"id":"p1200"},{"id":"p1198"},{"id":"p1199"}],"min_width":0,"margin":0,"sizing_mode":"stretch_width","align":"start"}},{"type":"object","name":"Figure","id":"p1209","attributes":{"width":700,"height":300,"margin":[5,10],"sizing_mode":"fixed","align":"start","x_range":{"type":"object","name":"Range1d","id":"p1202","attributes":{"tags":[[["DATE",null]],[]],"start":567993600000.0,"end":1767225600000.0,"reset_start":567993600000.0,"reset_end":1767225600000.0}},"y_range":{"type":"object","name":"Range1d","id":"p1203","attributes":{"tags":[[["temp_c",null]],{"type":"map","entries":[["invert_yaxis",false],["autorange",false]]}],"start":15.860508137220464,"end":21.625734691488116,"reset_start":15.860508137220464,"reset_end":21.625734691488116}},"x_scale":{"type":"object","name":"LinearScale","id":"p1219"},"y_scale":{"type":"object","name":"LinearScale","id":"p1220"},"title":{"type":"object","name":"Title","id":"p1212","attributes":{"text":"Mean Annual Temperature in SE Arizona","text_color":"black","text_font_size":"12pt"}},"renderers":[{"type":"object","name":"GlyphRenderer","id":"p1265","attributes":{"data_source":{"type":"object","name":"ColumnDataSource","id":"p1256","attributes":{"selected":{"type":"object","name":"Selection","id":"p1257","attributes":{"indices":[],"line_indices":[]}},"selection_policy":{"type":"object","name":"UnionRenderers","id":"p1258"},"data":{"type":"map","entries":[["DATE",{"type":"ndarray","array":{"type":"bytes","data":"H4sIAAEAAAAC/2NgYLj4sD3BiYGB4VBNcSKQbnheFJcE4vNmeiaD+EbxJikgWvmXfCpI3PMDVxqIn/fsK4hmmHLnQTqIbi0/kwESX5W7PRPEv5C8KAvE/xrZmw2in32pyAGJ87xOzgXxDR/65YH44dct80G0yk6hAiB9wMykA0Q3eK7/C6IdYrSKC0HiV76/KIS6rwgk/uvt5SKoO4tB4q1m+0G0w4yNJiUg8dU6q0D0gb3L5UtB4malU0uh7i8DiUdnN5RB/QGiGZ5vzi4Hif/UewiiG3hWhVWA9MmrngHRB6Z/cqyE+q/SCQDeVF/IOAEAAA=="},"shape":[39],"dtype":"float64","order":"little"}],["temp_c",{"type":"ndarray","array":{"type":"bytes","data":"H4sIAAEAAAAC/wE4Acf+LG10A77SNEC7IOyCsAsyQBupbqS6kTBAdAXSFUhXMEBm48emoZAwQANMXydjTzFAGZVRGZWRMUBevcedJIMxQIpNKTal2DFA7whaQWo8MUB5ueTlkpcwQBUqVKhQoTFA81z2ofIJMkAMwi4IuyAxQCwfsHzA8jFAJRGURFASMkAK7SW0l1AxQHfu3Llz5zFAYGp/qf2lMUB4DOAxgMcxQF3YcHZaZjFASQQlEZREMkA2FtdYXGMxQLGaw2oOqzFA1ySdQwNFMkA1adKkSZMxQN+EexPuTTJAylona52sMUCsuZqruRoyQMmtIreK3DJABvAYwGMAMkB8ou+JvicxQPK2iRYBlzJAqMGfBn8aMkCHtxneZngxQL/0S7/0SzJALjez8WNTMkCWD1g+YPkyQFMyJVMyJTVAVHPdaDgBAAA="},"shape":[39],"dtype":"float64","order":"little"}]]}}},"view":{"type":"object","name":"CDSView","id":"p1266","attributes":{"filter":{"type":"object","name":"AllIndices","id":"p1267"}}},"glyph":{"type":"object","name":"Line","id":"p1262","attributes":{"tags":["apply_ranges"],"x":{"type":"field","field":"DATE"},"y":{"type":"field","field":"temp_c"},"line_color":"#30a2da","line_width":2}},"selection_glyph":{"type":"object","name":"Line","id":"p1268","attributes":{"tags":["apply_ranges"],"x":{"type":"field","field":"DATE"},"y":{"type":"field","field":"temp_c"},"line_color":"#30a2da","line_width":2}},"nonselection_glyph":{"type":"object","name":"Line","id":"p1263","attributes":{"tags":["apply_ranges"],"x":{"type":"field","field":"DATE"},"y":{"type":"field","field":"temp_c"},"line_color":"#30a2da","line_alpha":0.1,"line_width":2}},"muted_glyph":{"type":"object","name":"Line","id":"p1264","attributes":{"tags":["apply_ranges"],"x":{"type":"field","field":"DATE"},"y":{"type":"field","field":"temp_c"},"line_color":"#30a2da","line_alpha":0.2,"line_width":2}}}}],"toolbar":{"type":"object","name":"Toolbar","id":"p1218","attributes":{"tools":[{"type":"object","name":"WheelZoomTool","id":"p1207","attributes":{"tags":["hv_created"],"renderers":"auto","zoom_together":"none"}},{"type":"object","name":"HoverTool","id":"p1208","attributes":{"tags":["hv_created"],"renderers":[{"id":"p1265"}],"tooltips":[["DATE","@{DATE}{%F %T}"],["temp_c","@{temp_c}"]],"formatters":{"type":"map","entries":[["@{DATE}","datetime"]]},"sort_by":null}},{"type":"object","name":"SaveTool","id":"p1245"},{"type":"object","name":"PanTool","id":"p1246"},{"type":"object","name":"BoxZoomTool","id":"p1247","attributes":{"dimensions":"both","overlay":{"type":"object","name":"BoxAnnotation","id":"p1248","attributes":{"syncable":false,"line_color":"black","line_alpha":1.0,"line_width":2,"line_dash":[4,4],"fill_color":"lightgrey","fill_alpha":0.5,"level":"overlay","visible":false,"left":{"type":"number","value":"nan"},"right":{"type":"number","value":"nan"},"top":{"type":"number","value":"nan"},"bottom":{"type":"number","value":"nan"},"left_units":"canvas","right_units":"canvas","top_units":"canvas","bottom_units":"canvas","handles":{"type":"object","name":"BoxInteractionHandles","id":"p1254","attributes":{"all":{"type":"object","name":"AreaVisuals","id":"p1253","attributes":{"fill_color":"white","hover_fill_color":"lightgray"}}}}}}}},{"type":"object","name":"ResetTool","id":"p1255"}],"active_drag":{"id":"p1246"},"active_scroll":{"id":"p1207"}}},"left":[{"type":"object","name":"LinearAxis","id":"p1240","attributes":{"ticker":{"type":"object","name":"BasicTicker","id":"p1241","attributes":{"mantissas":[1,2,5]}},"formatter":{"type":"object","name":"BasicTickFormatter","id":"p1242"},"axis_label":"Temperature (deg C)","major_label_policy":{"type":"object","name":"AllLabels","id":"p1243"}}}],"below":[{"type":"object","name":"DatetimeAxis","id":"p1221","attributes":{"ticker":{"type":"object","name":"DatetimeTicker","id":"p1222","attributes":{"num_minor_ticks":5,"tickers":[{"type":"object","name":"AdaptiveTicker","id":"p1223","attributes":{"num_minor_ticks":0,"mantissas":[1,2,5],"max_interval":500.0}},{"type":"object","name":"AdaptiveTicker","id":"p1224","attributes":{"num_minor_ticks":0,"base":60,"mantissas":[1,2,5,10,15,20,30],"min_interval":1000.0,"max_interval":1800000.0}},{"type":"object","name":"AdaptiveTicker","id":"p1225","attributes":{"num_minor_ticks":0,"base":24,"mantissas":[1,2,4,6,8,12],"min_interval":3600000.0,"max_interval":43200000.0}},{"type":"object","name":"DaysTicker","id":"p1226","attributes":{"days":[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31]}},{"type":"object","name":"DaysTicker","id":"p1227","attributes":{"days":[1,4,7,10,13,16,19,22,25,28]}},{"type":"object","name":"DaysTicker","id":"p1228","attributes":{"days":[1,8,15,22]}},{"type":"object","name":"DaysTicker","id":"p1229","attributes":{"days":[1,15]}},{"type":"object","name":"MonthsTicker","id":"p1230","attributes":{"months":[0,1,2,3,4,5,6,7,8,9,10,11]}},{"type":"object","name":"MonthsTicker","id":"p1231","attributes":{"months":[0,2,4,6,8,10]}},{"type":"object","name":"MonthsTicker","id":"p1232","attributes":{"months":[0,4,8]}},{"type":"object","name":"MonthsTicker","id":"p1233","attributes":{"months":[0,6]}},{"type":"object","name":"YearsTicker","id":"p1234"}]}},"formatter":{"type":"object","name":"DatetimeTickFormatter","id":"p1237","attributes":{"seconds":"%T","minsec":"%T","minutes":"%H:%M","hours":"%H:%M","days":"%b %d","months":"%b %Y","strip_leading_zeros":["microseconds","milliseconds","seconds"],"boundary_scaling":false,"context":{"type":"object","name":"DatetimeTickFormatter","id":"p1236","attributes":{"microseconds":"%T","milliseconds":"%T","seconds":"%b %d, %Y","minsec":"%b %d, %Y","minutes":"%b %d, %Y","hourmin":"%b %d, %Y","hours":"%b %d, %Y","days":"%Y","months":"","years":"","boundary_scaling":false,"hide_repeats":true,"context":{"type":"object","name":"DatetimeTickFormatter","id":"p1235","attributes":{"microseconds":"%b %d, %Y","milliseconds":"%b %d, %Y","seconds":"","minsec":"","minutes":"","hourmin":"","hours":"","days":"","months":"","years":"","boundary_scaling":false,"hide_repeats":true}},"context_which":"all"}},"context_which":"all"}},"axis_label":"Year","major_label_policy":{"type":"object","name":"AllLabels","id":"p1238"}}}],"center":[{"type":"object","name":"Grid","id":"p1239","attributes":{"axis":{"id":"p1221"},"grid_line_color":null}},{"type":"object","name":"Grid","id":"p1244","attributes":{"dimension":1,"axis":{"id":"p1240"},"grid_line_color":null}}],"min_border_top":10,"min_border_bottom":10,"min_border_left":10,"min_border_right":10,"output_backend":"webgl"}},{"type":"object","name":"Spacer","id":"p1270","attributes":{"name":"HSpacer01120","stylesheets":["\n:host(.pn-loading):before, .pn-loading:before {\n  background-color: #c3c3c3;\n  mask-size: auto calc(min(50%, 300px));\n  -webkit-mask-size: auto calc(min(50%, 300px));\n}",{"id":"p1200"},{"id":"p1198"},{"id":"p1199"}],"min_width":0,"margin":0,"sizing_mode":"stretch_width","align":"start"}}]}}],"defs":[{"type":"model","name":"ReactiveHTML1"},{"type":"model","name":"FlexBox1","properties":[{"name":"align_content","kind":"Any","default":"flex-start"},{"name":"align_items","kind":"Any","default":"flex-start"},{"name":"flex_direction","kind":"Any","default":"row"},{"name":"flex_wrap","kind":"Any","default":"wrap"},{"name":"gap","kind":"Any","default":""},{"name":"justify_content","kind":"Any","default":"flex-start"}]},{"type":"model","name":"FloatPanel1","properties":[{"name":"config","kind":"Any","default":{"type":"map"}},{"name":"contained","kind":"Any","default":true},{"name":"position","kind":"Any","default":"right-top"},{"name":"offsetx","kind":"Any","default":null},{"name":"offsety","kind":"Any","default":null},{"name":"theme","kind":"Any","default":"primary"},{"name":"status","kind":"Any","default":"normalized"}]},{"type":"model","name":"GridStack1","properties":[{"name":"ncols","kind":"Any","default":null},{"name":"nrows","kind":"Any","default":null},{"name":"allow_resize","kind":"Any","default":true},{"name":"allow_drag","kind":"Any","default":true},{"name":"state","kind":"Any","default":[]}]},{"type":"model","name":"drag1","properties":[{"name":"slider_width","kind":"Any","default":5},{"name":"slider_color","kind":"Any","default":"black"},{"name":"start","kind":"Any","default":0},{"name":"end","kind":"Any","default":100},{"name":"value","kind":"Any","default":50}]},{"type":"model","name":"click1","properties":[{"name":"terminal_output","kind":"Any","default":""},{"name":"debug_name","kind":"Any","default":""},{"name":"clears","kind":"Any","default":0}]},{"type":"model","name":"ReactiveESM1","properties":[{"name":"esm_constants","kind":"Any","default":{"type":"map"}}]},{"type":"model","name":"JSComponent1","properties":[{"name":"esm_constants","kind":"Any","default":{"type":"map"}}]},{"type":"model","name":"ReactComponent1","properties":[{"name":"use_shadow_dom","kind":"Any","default":true},{"name":"esm_constants","kind":"Any","default":{"type":"map"}}]},{"type":"model","name":"AnyWidgetComponent1","properties":[{"name":"use_shadow_dom","kind":"Any","default":true},{"name":"esm_constants","kind":"Any","default":{"type":"map"}}]},{"type":"model","name":"FastWrapper1","properties":[{"name":"object","kind":"Any","default":null},{"name":"style","kind":"Any","default":null}]},{"type":"model","name":"NotificationArea1","properties":[{"name":"js_events","kind":"Any","default":{"type":"map"}},{"name":"max_notifications","kind":"Any","default":5},{"name":"notifications","kind":"Any","default":[]},{"name":"position","kind":"Any","default":"bottom-right"},{"name":"_clear","kind":"Any","default":0},{"name":"types","kind":"Any","default":[{"type":"map","entries":[["type","warning"],["background","#ffc107"],["icon",{"type":"map","entries":[["className","fas fa-exclamation-triangle"],["tagName","i"],["color","white"]]}]]},{"type":"map","entries":[["type","info"],["background","#007bff"],["icon",{"type":"map","entries":[["className","fas fa-info-circle"],["tagName","i"],["color","white"]]}]]}]}]},{"type":"model","name":"Notification","properties":[{"name":"background","kind":"Any","default":null},{"name":"duration","kind":"Any","default":3000},{"name":"icon","kind":"Any","default":null},{"name":"message","kind":"Any","default":""},{"name":"notification_type","kind":"Any","default":null},{"name":"_rendered","kind":"Any","default":false},{"name":"_destroyed","kind":"Any","default":false}]},{"type":"model","name":"TemplateActions1","properties":[{"name":"open_modal","kind":"Any","default":0},{"name":"close_modal","kind":"Any","default":0}]},{"type":"model","name":"BootstrapTemplateActions1","properties":[{"name":"open_modal","kind":"Any","default":0},{"name":"close_modal","kind":"Any","default":0}]},{"type":"model","name":"TemplateEditor1","properties":[{"name":"layout","kind":"Any","default":[]}]},{"type":"model","name":"MaterialTemplateActions1","properties":[{"name":"open_modal","kind":"Any","default":0},{"name":"close_modal","kind":"Any","default":0}]},{"type":"model","name":"request_value1","properties":[{"name":"fill","kind":"Any","default":"none"},{"name":"_synced","kind":"Any","default":null},{"name":"_request_sync","kind":"Any","default":0}]}]}};
  var render_items = [{"docid":"9b2b1f88-4013-4700-9a09-132017edb0ce","roots":{"p1197":"f634fe9b-0226-4fcd-b82c-19ca37ce56d1"},"root_ids":["p1197"]}];
  var docs = Object.values(docs_json)
  if (!docs) {
    return
  }
  const py_version = docs[0].version.replace('rc', '-rc.').replace('.dev', '-dev.')
  async function embed_document(root) {
    var Bokeh = get_bokeh(root)
    await Bokeh.embed.embed_items_notebook(docs_json, render_items);
    for (const render_item of render_items) {
      for (const root_id of render_item.root_ids) {
	const id_el = document.getElementById(root_id)
	if (id_el.children.length && id_el.children[0].hasAttribute('data-root-id')) {
	  const root_el = id_el.children[0]
	  root_el.id = root_el.id + '-rendered'
	  for (const child of root_el.children) {
            // Ensure JupyterLab does not capture keyboard shortcuts
            // see: https://jupyterlab.readthedocs.io/en/4.1.x/extension/notebook.html#keyboard-interaction-model
	    child.setAttribute('data-lm-suppress-shortcuts', 'true')
	  }
	}
      }
    }
  }
  function get_bokeh(root) {
    if (root.Bokeh === undefined) {
      return null
    } else if (root.Bokeh.version !== py_version) {
      if (root.Bokeh.versions === undefined || !root.Bokeh.versions.has(py_version)) {
	return null
      }
      return root.Bokeh.versions.get(py_version);
    } else if (root.Bokeh.version === py_version) {
      return root.Bokeh
    }
    return null
  }
  function is_loaded(root) {
    var Bokeh = get_bokeh(root)
    return (Bokeh != null && Bokeh.Panel !== undefined)
  }
  if (is_loaded(root)) {
    embed_document(root);
  } else {
    var attempts = 0;
    var timer = setInterval(function(root) {
      if (is_loaded(root)) {
        clearInterval(timer);
        embed_document(root);
      } else if (document.readyState == "complete") {
        attempts++;
        if (attempts > 200) {
          clearInterval(timer);
	  var Bokeh = get_bokeh(root)
	  if (Bokeh == null || Bokeh.Panel == null) {
            console.warn("Panel: ERROR: Unable to run Panel code because Bokeh or Panel library is missing");
	  } else {
	    console.warn("Panel: WARNING: Attempting to render but not all required libraries could be resolved.")
	    embed_document(root)
	  }
        }
      }
    }, 25, root)
  }
})(window);</script>



>**Data Exploration**
>If we ignore years with incomplete data:
>* The minimum mean annual temperature is 16.341 degrees C in 1991
>* The maximum mean annual temperature is 18.974 degrees C in 2025

## Quantify how fast the climate is changing with a trend line

    Slope: [0.03525516] degrees per year


### Plot your trend line

Trend lines are often used to help your audience understand and process
a time-series plot. In this case, we’ve chosen mean temperature values
rather than extremes, so we think OLS is an appropriate model to use to
show a trend.


    
![png](climate-change_files/climate-change_27_0.png)
    


>*Mean annual temperatures in Boulder, CO have increased over the last century*

>In SE Arizona, mean annual temperatures have increased by 0.035 degrees C per year from 1989 to 2025. Temperatures are likely increasing as a result of climate change, although other environmental characteristics, like trends in sea surface temperatures, may also influence some of this rate of temperature change.
