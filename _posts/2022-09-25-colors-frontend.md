---
toc: false
layout: post
categories: [markdown]
title: Colors Frontend
comments: true
---

<table>
  <thead>
  <tr>
    <th>Name</th>
    <th>Emotion</th>
    <th>Symbolism</th>
  </tr>
  </thead>
  <tbody id="result">
  </tbody>
</table>

<script>
    const resultContainer = document.getElementById("result");

   // function holds data for colors
    function Color(name, emotion, symbolism) {
        this.name = name;
        this.emotion = emotion;
        this.symbolism = symbolism;
    }

    // json conversion function
    Color.prototype.toJSON = function() {
        const obj = {name: this.name, emotion: this.emotion, symbolism: this.symbolism};
        const json = JSON.stringify(obj);
        return json;
    }

    // list of colors
    var list = [ 
        new Color( "Red", ":)", "life, health, vigor"),
        new Color( "Orange", ":)", "fun, strength, courage"),
        new Color( "Yellow", ":)", "happiness, warmth, sunshine"),
        new Color( "Green", ":|", "nature, wisdom"),
        new Color( "Blue", ":(", "calmness, despair"),
        new Color( "Indigo", ":(", "communication, peace"),
        new Color( "Violet", ":(", "higher self, comprehension")
    ];

    function ColorClass(colors){
        this.ColorClass = colors;
        this.json = [];
        this.ColorClass.forEach(colors => this.json.push(colors.toJSON()));
    }

    // creates colorlist object
    colorlist = new ColorClass(list);

// javascript variables and methods to build html using previous data

    for (const row of colorlist.ColorClass) {

        const tr = document.createElement("tr");

        const name = document.createElement("td");
        const emotion = document.createElement("td");
        const symbolism = document.createElement("td");

        name.innerHTML = row.emotion;
        emotion.innerHTML = row.symbolism; 
        symbolism.innerHTML = row.name; 


        tr.appendChild(symbolism);
        tr.appendChild(name);
        tr.appendChild(emotion);


        resultContainer.appendChild(tr);
    }
</script>