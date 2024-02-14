---
permalink: /test/
title: "Test"
datatable: true
---

|First Header | Second Header|
|------------ | -------------|
|Content from cell 1 | Content from cell 2|
|Content in the first column | Content in the second column|
{:.wide}

|First Header | Second Header|
|------------ | -------------|
|Content from cell 1 | Content from cell 2|
|Content in the first column | Content in the second column|
{:.inner-borders}

|---
| Default aligned | Left aligned | Center aligned | Right aligned
|-|:-|:-:|-:
| First body part | Second cell | Third cell | fourth cell
| Second line |foo | **strong** | baz
| Third line |quux | baz | bar
|---
| Second body
| 2 line
|===
| Footer row

<div class="datatable-begin"></div>

Food    | Description                           | Category | Sample type
------- | ------------------------------------- | -------- | -----------
Apples  | A small, somewhat round ...           | Fruit    | Fuji
Bananas | A long and curved, often-yellow ...   | Fruit    | Snow
Kiwis   | A small, hairy-skinned sweet ...      | Fruit    | Golden
Oranges | A spherical, orange-colored sweet ... | Fruit    | Navel

<div class="datatable-end"></div>

<table class="display">
<thead>
<tr class="header">
<th>Bass Weapon</th>
<th></th>
<th>Passive item</th>
<th></th>
<th>Evolution</th>
</tr>
</thead>
<tbody>
{% for item in site.data.evolutions %}
  <tr style="border-bottom: 1px;">
    <td><img src="{{ item.base_weapon }}" height="32"/></td>
    <td>+</td>
    <td><img src="{{ item.passive_item }}" height="32"/></td>
    <td>=</td>
    <td><img src="{{ item.evolution }}" height="32"/></td>
  </tr>
{% endfor %}
</tbody>
</table>
{:.vs-weapons}
