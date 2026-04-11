## Minecraft load time benchmark

---

<p align="center" style="font-size:160%;">
MC total load time:<br>
292 sec
<br>
<sup><sub>(
4:52 min
)</sub></sup>
</p>

<br>
<!--
Note for image scripts:
  - Newlines are ignored
  - This characters cant be used: +<"%#
-->
<p align="center">
<img src="https://quickchart.io/chart.png?w=400&h=60&c={
  type: 'horizontalBar',
  data: {
    datasets: [
        {label: 'Mixins\n', data: [33.00]},
        {label: 'Construction\n', data: [65.00]},
        {label: 'PreInit\n', data: [136.00]},
        {label: 'Init\n', data: [55.00]},
    ]
  },
  options: {
    layout: { padding: { top: 10 } },
    scales: {
      xAxes: [{display: false, stacked: true}],
      yAxes: [{display: false, stacked: true}],
    },
    elements: {rectangle: {borderWidth: 2}},
    legend: {display: false},
    plugins: {datalabels: {
      color: 'white',
      font: {
        family: 'Consolas',
      },
      formatter: (value, context) =>
        [context.dataset.label, value, 's'].join('')
    }},
    annotation: {
      clip: false,
      annotations: [{
          type: 'line',
          scaleID: 'x-axis-0',
          value: 33,
          borderColor: 'black',
          label: {
            content: 'Window appear',
            fontSize: 8,
            enabled: true,
            xPadding: 8, yPadding: 2,
            yAdjust: -20
          },
        }
      ]
    },
  }
}"/>
</p>

<br>

# Mods Loading Time

<p align="center">
<img src="https://quickchart.io/chart.png?w=400&h=300&c={
  type: 'outlabeledPie',
  options: {
    rotation: Math.PI,
    cutoutPercentage: 25,
    plugins: {
      legend: !1,
      outlabels: {
        stretch: 5,
        padding: 1,
        text: (v,i)=>[
          v.labels[v.dataIndex],' ',
          (v.percent*1000|0)/10,
          String.fromCharCode(37)].join('')
      }
    }
  },
  data: {...
`
436e17  8.62s Had Enough Items;
395E14  0.73s [JEI Ingredient Filter];
395E14  6.86s [JEI Plugins];
5161a8  7.87s CraftTweaker2;
516fa8  6.40s Ender IO;
8f304e  5.83s Astral Sorcery;
a651a8  5.10s IndustrialCraft 2;
6e5e17  4.66s Tinkers' Antique;
5E5014  3.00s [TCon Textures];
cd922c  3.83s NuclearCraft;
813e81  3.49s OpenComputers;
6e175e  3.20s Recurrent Complex;
213664  3.09s Forestry;
308f7e  2.34s Quark: RotN Edition;
436e17  2.25s Integrated Dynamics;
ba3eb8  2.20s Cyclic;
306e8f  2.13s Custom Loading Screen;
308f53  2.10s Village Names;
813e80  2.09s Shadowfacts' Forgelin (Dummy);
444444 36.35s 23 Other mods;
333333 48.30s 152 'Fast' mods (1.0s - 0.1s);
222222  8.02s 303 'Instant' mods (%3C 0.1s)
`
    .split(';').reduce((a, l) => {
      l.match(/(\w{6}) *(\d*\.\d*) ?s (.*)/s)
      .slice(1).map((a, i) => [[String.fromCharCode(35),a].join(''), a,
        a.length > 15 ? a.split(/(?%3C=.{9})\s(?=\S{5})/).join('\n') : a
      ][i])
      .forEach((s, i) =>
        [a.datasets[0].backgroundColor, a.datasets[0].data, a.labels][i].push(s)
      );
      return a
    }, {
      labels: [],
      datasets: [{
        backgroundColor: [],
        data: [],
        borderColor: 'rgba(22,22,22,0.3)',
        borderWidth: 1
      }]
    })
  }
}"/>
</p>

<br>

# Loader steps

Show how much time each mod takes on each game load phase.

JEI/HEI not included, since its load time based on other mods and overal item count.

<p align="center">
<img src="https://quickchart.io/chart.png?w=400&h=450&c={
  options: {
    scales: {
      xAxes: [{stacked: true}],
      yAxes: [{stacked: true}],
    },
    plugins: {
      datalabels: {
        anchor: 'end',
        align: 'top',
        color: 'white',
        backgroundColor: 'rgba(46, 140, 171, 0.6)',
        borderColor: 'rgba(41, 168, 194, 1.0)',
        borderWidth: 0.5,
        borderRadius: 3,
        padding: 0,
        font: {size:10},
        formatter: (v,ctx) =>
          ctx.datasetIndex!=ctx.chart.data.datasets.length-1 ? null
            : [((ctx.chart.data.datasets.reduce((a,b)=>a- -b.data[ctx.dataIndex],0)*10)|0)/10,'s'].join('')
      },
      colorschemes: {
        scheme: 'office.Damask6'
      }
    }
  },
  type: 'bar',
  data: {...(() => {
    let a = { labels: [], datasets: [] };
`
0: Construction;
1: Loading Resources;
2: PreInitialization;
3: Initialization;
4: InterModComms;
5: LoadComplete;
6: ModIdMapping;
7: Other
`
    .split(';')
      .map(l => l.match(/\d: (.*)/).slice(1))
      .forEach(([name]) => a.datasets.push({ label: name, data: [] }));
`
                                  0      1      2      3      4      5      6      7;
CraftTweaker2                 | 0.22| 0.00| 2.99| 4.61| 0.00| 0.05| 0.00| 0.00;
Ender IO                      | 1.67| 0.01| 2.83| 0.30| 1.58| 0.00| 0.01| 0.00;
Astral Sorcery                | 0.17| 0.00| 4.49| 1.17| 0.00| 0.00| 0.00| 0.00;
IndustrialCraft 2             | 0.91| 0.01| 3.44| 0.75| 0.00| 0.00| 0.00| 0.00;
Tinkers' Antique              | 1.00| 0.01| 0.11| 0.55| 0.00| 0.00| 0.00| 3.00;
NuclearCraft                  | 0.05| 0.01| 2.96| 0.79| 0.00| 0.00| 0.03| 0.00;
OpenComputers                 | 0.15| 0.01| 1.40| 1.87| 0.07| 0.00| 0.00| 0.00;
Recurrent Complex             | 0.18| 0.00| 0.29| 2.72| 0.00| 0.00| 0.00| 0.00;
Forestry                      | 0.33| 0.01| 2.13| 0.63| 0.00| 0.00| 0.00| 0.00;
Quark: RotN Edition           | 0.02| 0.01| 2.20| 0.11| 0.00| 0.00| 0.00| 0.00;
[Mod Average]                 | 0.07| 0.00| 0.16| 0.08| 0.00| 0.00| 0.00| 0.01
`
    .split(';').slice(1)
      .map(l => l.split('|').map(s => s.trim()))
      .forEach(([name, ...arr], i) => {
        a.labels.push(name);
        arr.forEach((v, j) => a.datasets[j].data[i] = v)
      }); return a
  })()}
}"/>
</p>

<br>

# TOP JEI Registered Plugis

<p align="center">
<img src="https://quickchart.io/chart.png?w=500&h=200&c={
  options: {
    elements: { rectangle: { borderWidth: 1 } },
    legend: false,
    scales: {
      yAxes: [{ ticks: { fontSize: 9, fontFamily: 'Verdana' }}],
    },
  },
  type: 'horizontalBar',
    data: {...(() => {
      let a = {
        labels: [], datasets: [{
          backgroundColor: 'rgba(0, 99, 132, 0.5)',
          borderColor: 'rgb(0, 99, 132)',
          data: []
        }]
      };
`
 1.03: li.cil.oc.integration.jei.ModPluginOpenComputers;
 0.76: jeresources.jei.JEIConfig;
 0.69: com.rwtema.extrautils2.crafting.jei.XUJEIPlugin;
 0.56: com.buuz135.industrial.jei.JEICustomPlugin;
 0.46: crazypants.enderio.machines.integration.jei.MachinesPlugin;
 0.45: mezz.jei.plugins.vanilla.VanillaPlugin;
 0.41: knightminer.tcomplement.plugin.jei.JEIPlugin;
 0.36: ic2.jeiIntegration.SubModule;
 0.17: cofh.thermalexpansion.plugins.jei.JEIPluginTE;
 0.17: crazypants.enderio.base.integration.jei.JeiPlugin;
 0.16: com.buuz135.thaumicjei.ThaumcraftJEIPlugin;
 0.10: net.bdew.jeibees.BeesJEIPlugin;
 1.54: Other
`
        .split(';')
        .map(l => l.split(':'))
        .forEach(([time, name]) => {
          a.labels.push(name);
          a.datasets[0].data.push(time)
        })
        ; return a
    })()
  }
}"/>
</p>

<br>

# FML Stuff

Loading bars that usually not related to specific mods.

⚠️ Shows only steps that took 1.0 sec or more.

<p align="center">
<img src="https://quickchart.io/chart.png?w=500&h=400&c={
  options: {
    rotation: Math.PI*1.125,
    cutoutPercentage: 55,
    plugins: {
      legend: !1,
      outlabels: {
        stretch: 5,
        padding: 1,
        text: (v)=>v.labels
      },
      doughnutlabel: {
        labels: [
          {
            text: 'FML stuff:',
            color: 'rgba(128, 128, 128, 0.5)',
            font: {size: 18}
          },
          {
            text: '123.70s',
            color: 'rgba(128, 128, 128, 1)',
            font: {size: 22}
          }
        ]
      },
    }
  },
  type: 'outlabeledPie',
  data: {...(() => {
    let a = {
      labels: [],
      datasets: [{
        backgroundColor: [],
        data: [],
        borderColor: 'rgba(22,22,22,0.3)',
        borderWidth: 2
      }]
    };
`
994400  1.56s Reloading;
001799  2.60s Loading Resource - AssetLibrary;
179900  3.80s Preloading 53255 textures;
0D9900  1.79s Texture loading;
009911  1.79s Texture mipmap and upload;
009926  5.27s Posting bake events;
009930 33.07s Setting up dynamic models;
00993A 33.16s Loading Resource - ModelManager;
009299 33.95s Rendering Setup;
590099  1.53s XML Recipes;
630099  2.08s InterModComms;
990040 12.46s [VintageFix]: Texture search 69841 sprites;
990036  3.91s Preloaded 33665 sprites
`
    .split(';')
      .map(l => l.match(/(\w{6}) *(\d*\.\d*) ?s (.*)/s))
      .forEach(([, col, time, name]) => {
        a.labels.push([
          name.length > 15 ? name.split(/(?%3C=.{11})\s(?=\S{6})/).join('\n') : name
          , ' ', time, 's'
        ].join(''));
        a.datasets[0].data.push(parseFloat(time));
        a.datasets[0].backgroundColor.push([String.fromCharCode(35), col].join(''))
      })
      ; return a
  })()}
}"/>
</p>
