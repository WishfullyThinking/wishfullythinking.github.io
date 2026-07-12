---
layout: post
title: Late Surgers Like Fast Races, and Other Half-Truths
output:
  md_document:
    variant: markdown_github
    preserve_yaml: true
---

### Introduction

A classic piece of horseracing wisdom goes like this: if the pace is
great, surge late; if the leader is a snail, stay on their tail.

In other words, if the frontrunners go full-throttle at the start of the
race, those attempting to match the pace tire themselves out by the home
stretch and become easy pickings for the surgers and the closers.
Conversely, if the frontrunners set a slow pace, then everyone is fresh
enough to mount a late challenge, favouring the runners closer to the
front.

This effect — so goes the traditional wisdom — is magnified or
diminished by certain racecourses. Tokyo’s enormous 525m of unbroken
final straight allows for improbable catch-ups: a classic example is the
2022 Tenno Sho Autumn, where Panthalassa was leading by 15 lengths at
the final turn but was caught by Equinox close to the wire. On the other
hand, Hanshin is [notoriously
favourable](https://idolhorse.com/horse-racing-news/japan/g1-guide-tips-osaka-hai/#:~:text=Hanshin's%202000m%20is%20quite%20a%20biased%20track,behind%20the%20leaders%20will%20have%20an%20advantage.)
to those towards the front. Even the habitual closer Gold Ship was raced
ahead in both his Takarazuka conquests.

Can we check is this common sense is empirically true? As it happens,
for a rough guess at the truth, the statistical data comes almost
ready-made.

### Sectional Times: How Fast was the Early Pace?

Those who know how to read sectional times can skip ahead to the next
section.

How fast the front-runners are going can be quantified by *sectional
data*. For a given race, the sectionals measure the time it took for the
leading horse in the race to reach 200m, 400m, and so on.

<div id="kopyrseemk" style="padding-left:0px;padding-right:0px;padding-top:10px;padding-bottom:10px;overflow-x:auto;overflow-y:auto;width:auto;height:auto;">
<style>#kopyrseemk table {
  font-family: system-ui, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol', 'Noto Color Emoji';
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

#kopyrseemk thead, #kopyrseemk tbody, #kopyrseemk tfoot, #kopyrseemk tr, #kopyrseemk td, #kopyrseemk th {
  border-style: none;
}

#kopyrseemk p {
  margin: 0;
  padding: 0;
}

#kopyrseemk .gt_table {
  display: table;
  border-collapse: collapse;
  line-height: normal;
  margin-left: auto;
  margin-right: auto;
  color: #333333;
  font-size: 16px;
  font-weight: normal;
  font-style: normal;
  background-color: #FFFFFF;
  width: auto;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #A8A8A8;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #A8A8A8;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
}

#kopyrseemk .gt_caption {
  padding-top: 4px;
  padding-bottom: 4px;
}

#kopyrseemk .gt_title {
  color: #333333;
  font-size: 125%;
  font-weight: initial;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-color: #FFFFFF;
  border-bottom-width: 0;
}

#kopyrseemk .gt_subtitle {
  color: #333333;
  font-size: 85%;
  font-weight: initial;
  padding-top: 3px;
  padding-bottom: 5px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-color: #FFFFFF;
  border-top-width: 0;
}

#kopyrseemk .gt_heading {
  background-color: #FFFFFF;
  text-align: center;
  border-bottom-color: #FFFFFF;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#kopyrseemk .gt_bottom_border {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#kopyrseemk .gt_col_headings {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#kopyrseemk .gt_col_heading {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  overflow-x: hidden;
}

#kopyrseemk .gt_column_spanner_outer {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  padding-top: 0;
  padding-bottom: 0;
  padding-left: 4px;
  padding-right: 4px;
}

#kopyrseemk .gt_column_spanner_outer:first-child {
  padding-left: 0;
}

#kopyrseemk .gt_column_spanner_outer:last-child {
  padding-right: 0;
}

#kopyrseemk .gt_column_spanner {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 5px;
  overflow-x: hidden;
  display: inline-block;
  width: 100%;
}

#kopyrseemk .gt_spanner_row {
  border-bottom-style: hidden;
}

#kopyrseemk .gt_group_heading {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  text-align: left;
}

#kopyrseemk .gt_empty_group_heading {
  padding: 0.5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: middle;
}

#kopyrseemk .gt_from_md > :first-child {
  margin-top: 0;
}

#kopyrseemk .gt_from_md > :last-child {
  margin-bottom: 0;
}

#kopyrseemk .gt_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  margin: 10px;
  border-top-style: solid;
  border-top-width: 1px;
  border-top-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  overflow-x: hidden;
}

#kopyrseemk .gt_stub {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
}

#kopyrseemk .gt_stub_row_group {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
  vertical-align: top;
}

#kopyrseemk .gt_row_group_first td {
  border-top-width: 2px;
}

#kopyrseemk .gt_row_group_first th {
  border-top-width: 2px;
}

#kopyrseemk .gt_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#kopyrseemk .gt_first_summary_row {
  border-top-style: solid;
  border-top-color: #D3D3D3;
}

#kopyrseemk .gt_first_summary_row.thick {
  border-top-width: 2px;
}

#kopyrseemk .gt_last_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#kopyrseemk .gt_grand_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#kopyrseemk .gt_first_grand_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: double;
  border-top-width: 6px;
  border-top-color: #D3D3D3;
}

#kopyrseemk .gt_last_grand_summary_row_top {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: double;
  border-bottom-width: 6px;
  border-bottom-color: #D3D3D3;
}

#kopyrseemk .gt_striped {
  background-color: rgba(128, 128, 128, 0.05);
}

#kopyrseemk .gt_table_body {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#kopyrseemk .gt_footnotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#kopyrseemk .gt_footnote {
  margin: 0px;
  font-size: 90%;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}

#kopyrseemk .gt_sourcenotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#kopyrseemk .gt_sourcenote {
  font-size: 90%;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}

#kopyrseemk .gt_left {
  text-align: left;
}

#kopyrseemk .gt_center {
  text-align: center;
}

#kopyrseemk .gt_right {
  text-align: right;
  font-variant-numeric: tabular-nums;
}

#kopyrseemk .gt_font_normal {
  font-weight: normal;
}

#kopyrseemk .gt_font_bold {
  font-weight: bold;
}

#kopyrseemk .gt_font_italic {
  font-style: italic;
}

#kopyrseemk .gt_super {
  font-size: 65%;
}

#kopyrseemk .gt_footnote_marks {
  font-size: 75%;
  vertical-align: 0.4em;
  position: initial;
}

#kopyrseemk .gt_asterisk {
  font-size: 100%;
  vertical-align: 0;
}

#kopyrseemk .gt_indent_1 {
  text-indent: 5px;
}

#kopyrseemk .gt_indent_2 {
  text-indent: 10px;
}

#kopyrseemk .gt_indent_3 {
  text-indent: 15px;
}

#kopyrseemk .gt_indent_4 {
  text-indent: 20px;
}

#kopyrseemk .gt_indent_5 {
  text-indent: 25px;
}

#kopyrseemk .katex-display {
  display: inline-flex !important;
  margin-bottom: 0.75em !important;
}

#kopyrseemk div.Reactable > div.rt-table > div.rt-thead > div.rt-tr.rt-tr-group-header > div.rt-th-group:after {
  height: 0px !important;
}
</style>
<table class="gt_table" data-quarto-disable-processing="false" data-quarto-bootstrap="false">
  <thead>
    <tr class="gt_heading">
      <td colspan="3" class="gt_heading gt_title gt_font_normal gt_bottom_border" style>Sectional Times for the 2022 TENNO SHO (AUTUMN)</td>
    </tr>
    
    <tr class="gt_col_headings">
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Sectional-Distance-(m)">Sectional Distance (m)</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Sectional-Time-(s)">Sectional Time (s)</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Total-Time-(m:s)">Total Time (m:s)</th>
    </tr>
  </thead>
  <tbody class="gt_table_body">
    <tr><td headers="Sectional Distance (m)" class="gt_row gt_right">200</td>
<td headers="Sectional Time (s)" class="gt_row gt_right">12.6</td>
<td headers="Total Time (m:s)" class="gt_row gt_right">0:12.6</td></tr>
    <tr><td headers="Sectional Distance (m)" class="gt_row gt_right">400</td>
<td headers="Sectional Time (s)" class="gt_row gt_right">10.9</td>
<td headers="Total Time (m:s)" class="gt_row gt_right">0:23.5</td></tr>
    <tr><td headers="Sectional Distance (m)" class="gt_row gt_right">600</td>
<td headers="Sectional Time (s)" class="gt_row gt_right">11.2</td>
<td headers="Total Time (m:s)" class="gt_row gt_right">0:34.7</td></tr>
    <tr><td headers="Sectional Distance (m)" class="gt_row gt_right">800</td>
<td headers="Sectional Time (s)" class="gt_row gt_right">11.3</td>
<td headers="Total Time (m:s)" class="gt_row gt_right">0:46.0</td></tr>
    <tr><td headers="Sectional Distance (m)" class="gt_row gt_right">1000</td>
<td headers="Sectional Time (s)" class="gt_row gt_right">11.4</td>
<td headers="Total Time (m:s)" class="gt_row gt_right">0:57.4</td></tr>
    <tr><td headers="Sectional Distance (m)" class="gt_row gt_right">1200</td>
<td headers="Sectional Time (s)" class="gt_row gt_right">11.6</td>
<td headers="Total Time (m:s)" class="gt_row gt_right">1:09.0</td></tr>
    <tr><td headers="Sectional Distance (m)" class="gt_row gt_right">1400</td>
<td headers="Sectional Time (s)" class="gt_row gt_right">11.8</td>
<td headers="Total Time (m:s)" class="gt_row gt_right">1:20.8</td></tr>
    <tr><td headers="Sectional Distance (m)" class="gt_row gt_right">1600</td>
<td headers="Sectional Time (s)" class="gt_row gt_right">11.6</td>
<td headers="Total Time (m:s)" class="gt_row gt_right">1:32.4</td></tr>
    <tr><td headers="Sectional Distance (m)" class="gt_row gt_right">1800</td>
<td headers="Sectional Time (s)" class="gt_row gt_right">12.4</td>
<td headers="Total Time (m:s)" class="gt_row gt_right">1:44.8</td></tr>
    <tr><td headers="Sectional Distance (m)" class="gt_row gt_right">2000</td>
<td headers="Sectional Time (s)" class="gt_row gt_right">12.7</td>
<td headers="Total Time (m:s)" class="gt_row gt_right">1:57.5</td></tr>
  </tbody>
  
</table>
</div>

This table can be read as follows. When the leading horse completed the
first 200m, 12.6 seconds had elapsed. 10.9 seconds later, the leading
horse reached the 400m point. Note that it doesn’t have to be the same
horse. It can be the case that the leader at 200m was not the leader at
400m. Sectional times measure the speed of the *race*, not any
particular horse.

What do the numbers tell us? In general, if the turf isn’t too soft,
sectional times of 12 seconds or so are “normal”. Sectionals below 12
seconds are fast, above it are slow. This particular race, then,
featured extremely rapid sectionals for nearly the whole race. It was,
of course, Panthalassa’s famous getaway — foiled just in time by
Equinox.

Conversely, here’s another race at Fuchu which featured a getaway, this
time a successful one:

<div id="zyyeyernho" style="padding-left:0px;padding-right:0px;padding-top:10px;padding-bottom:10px;overflow-x:auto;overflow-y:auto;width:auto;height:auto;">
<style>#zyyeyernho table {
  font-family: system-ui, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol', 'Noto Color Emoji';
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

#zyyeyernho thead, #zyyeyernho tbody, #zyyeyernho tfoot, #zyyeyernho tr, #zyyeyernho td, #zyyeyernho th {
  border-style: none;
}

#zyyeyernho p {
  margin: 0;
  padding: 0;
}

#zyyeyernho .gt_table {
  display: table;
  border-collapse: collapse;
  line-height: normal;
  margin-left: auto;
  margin-right: auto;
  color: #333333;
  font-size: 16px;
  font-weight: normal;
  font-style: normal;
  background-color: #FFFFFF;
  width: auto;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #A8A8A8;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #A8A8A8;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
}

#zyyeyernho .gt_caption {
  padding-top: 4px;
  padding-bottom: 4px;
}

#zyyeyernho .gt_title {
  color: #333333;
  font-size: 125%;
  font-weight: initial;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-color: #FFFFFF;
  border-bottom-width: 0;
}

#zyyeyernho .gt_subtitle {
  color: #333333;
  font-size: 85%;
  font-weight: initial;
  padding-top: 3px;
  padding-bottom: 5px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-color: #FFFFFF;
  border-top-width: 0;
}

#zyyeyernho .gt_heading {
  background-color: #FFFFFF;
  text-align: center;
  border-bottom-color: #FFFFFF;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#zyyeyernho .gt_bottom_border {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#zyyeyernho .gt_col_headings {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#zyyeyernho .gt_col_heading {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  overflow-x: hidden;
}

#zyyeyernho .gt_column_spanner_outer {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  padding-top: 0;
  padding-bottom: 0;
  padding-left: 4px;
  padding-right: 4px;
}

#zyyeyernho .gt_column_spanner_outer:first-child {
  padding-left: 0;
}

#zyyeyernho .gt_column_spanner_outer:last-child {
  padding-right: 0;
}

#zyyeyernho .gt_column_spanner {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 5px;
  overflow-x: hidden;
  display: inline-block;
  width: 100%;
}

#zyyeyernho .gt_spanner_row {
  border-bottom-style: hidden;
}

#zyyeyernho .gt_group_heading {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  text-align: left;
}

#zyyeyernho .gt_empty_group_heading {
  padding: 0.5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: middle;
}

#zyyeyernho .gt_from_md > :first-child {
  margin-top: 0;
}

#zyyeyernho .gt_from_md > :last-child {
  margin-bottom: 0;
}

#zyyeyernho .gt_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  margin: 10px;
  border-top-style: solid;
  border-top-width: 1px;
  border-top-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  overflow-x: hidden;
}

#zyyeyernho .gt_stub {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
}

#zyyeyernho .gt_stub_row_group {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
  vertical-align: top;
}

#zyyeyernho .gt_row_group_first td {
  border-top-width: 2px;
}

#zyyeyernho .gt_row_group_first th {
  border-top-width: 2px;
}

#zyyeyernho .gt_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#zyyeyernho .gt_first_summary_row {
  border-top-style: solid;
  border-top-color: #D3D3D3;
}

#zyyeyernho .gt_first_summary_row.thick {
  border-top-width: 2px;
}

#zyyeyernho .gt_last_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#zyyeyernho .gt_grand_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#zyyeyernho .gt_first_grand_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: double;
  border-top-width: 6px;
  border-top-color: #D3D3D3;
}

#zyyeyernho .gt_last_grand_summary_row_top {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: double;
  border-bottom-width: 6px;
  border-bottom-color: #D3D3D3;
}

#zyyeyernho .gt_striped {
  background-color: rgba(128, 128, 128, 0.05);
}

#zyyeyernho .gt_table_body {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#zyyeyernho .gt_footnotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#zyyeyernho .gt_footnote {
  margin: 0px;
  font-size: 90%;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}

#zyyeyernho .gt_sourcenotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#zyyeyernho .gt_sourcenote {
  font-size: 90%;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}

#zyyeyernho .gt_left {
  text-align: left;
}

#zyyeyernho .gt_center {
  text-align: center;
}

#zyyeyernho .gt_right {
  text-align: right;
  font-variant-numeric: tabular-nums;
}

#zyyeyernho .gt_font_normal {
  font-weight: normal;
}

#zyyeyernho .gt_font_bold {
  font-weight: bold;
}

#zyyeyernho .gt_font_italic {
  font-style: italic;
}

#zyyeyernho .gt_super {
  font-size: 65%;
}

#zyyeyernho .gt_footnote_marks {
  font-size: 75%;
  vertical-align: 0.4em;
  position: initial;
}

#zyyeyernho .gt_asterisk {
  font-size: 100%;
  vertical-align: 0;
}

#zyyeyernho .gt_indent_1 {
  text-indent: 5px;
}

#zyyeyernho .gt_indent_2 {
  text-indent: 10px;
}

#zyyeyernho .gt_indent_3 {
  text-indent: 15px;
}

#zyyeyernho .gt_indent_4 {
  text-indent: 20px;
}

#zyyeyernho .gt_indent_5 {
  text-indent: 25px;
}

#zyyeyernho .katex-display {
  display: inline-flex !important;
  margin-bottom: 0.75em !important;
}

#zyyeyernho div.Reactable > div.rt-table > div.rt-thead > div.rt-tr.rt-tr-group-header > div.rt-th-group:after {
  height: 0px !important;
}
</style>
<table class="gt_table" data-quarto-disable-processing="false" data-quarto-bootstrap="false">
  <thead>
    <tr class="gt_heading">
      <td colspan="3" class="gt_heading gt_title gt_font_normal gt_bottom_border" style>Sectional Times for the 2003 JAPAN CUP</td>
    </tr>
    
    <tr class="gt_col_headings">
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Sectional-Distance-(m)">Sectional Distance (m)</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Sectional-Time-(s)">Sectional Time (s)</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Total-Time-(m:s)">Total Time (m:s)</th>
    </tr>
  </thead>
  <tbody class="gt_table_body">
    <tr><td headers="Sectional Distance (m)" class="gt_row gt_right">200</td>
<td headers="Sectional Time (s)" class="gt_row gt_right">12.9</td>
<td headers="Total Time (m:s)" class="gt_row gt_right">0:12.9</td></tr>
    <tr><td headers="Sectional Distance (m)" class="gt_row gt_right">400</td>
<td headers="Sectional Time (s)" class="gt_row gt_right">11.7</td>
<td headers="Total Time (m:s)" class="gt_row gt_right">0:24.6</td></tr>
    <tr><td headers="Sectional Distance (m)" class="gt_row gt_right">600</td>
<td headers="Sectional Time (s)" class="gt_row gt_right">13.1</td>
<td headers="Total Time (m:s)" class="gt_row gt_right">0:37.7</td></tr>
    <tr><td headers="Sectional Distance (m)" class="gt_row gt_right">800</td>
<td headers="Sectional Time (s)" class="gt_row gt_right">12.4</td>
<td headers="Total Time (m:s)" class="gt_row gt_right">0:50.1</td></tr>
    <tr><td headers="Sectional Distance (m)" class="gt_row gt_right">1000</td>
<td headers="Sectional Time (s)" class="gt_row gt_right">11.8</td>
<td headers="Total Time (m:s)" class="gt_row gt_right">1:01.9</td></tr>
    <tr><td headers="Sectional Distance (m)" class="gt_row gt_right">1200</td>
<td headers="Sectional Time (s)" class="gt_row gt_right">12.2</td>
<td headers="Total Time (m:s)" class="gt_row gt_right">1:14.1</td></tr>
    <tr><td headers="Sectional Distance (m)" class="gt_row gt_right">1400</td>
<td headers="Sectional Time (s)" class="gt_row gt_right">12.2</td>
<td headers="Total Time (m:s)" class="gt_row gt_right">1:26.3</td></tr>
    <tr><td headers="Sectional Distance (m)" class="gt_row gt_right">1600</td>
<td headers="Sectional Time (s)" class="gt_row gt_right">12.8</td>
<td headers="Total Time (m:s)" class="gt_row gt_right">1:39.1</td></tr>
    <tr><td headers="Sectional Distance (m)" class="gt_row gt_right">1800</td>
<td headers="Sectional Time (s)" class="gt_row gt_right">12.2</td>
<td headers="Total Time (m:s)" class="gt_row gt_right">1:51.3</td></tr>
    <tr><td headers="Sectional Distance (m)" class="gt_row gt_right">2000</td>
<td headers="Sectional Time (s)" class="gt_row gt_right">12.0</td>
<td headers="Total Time (m:s)" class="gt_row gt_right">2:03.3</td></tr>
    <tr><td headers="Sectional Distance (m)" class="gt_row gt_right">2200</td>
<td headers="Sectional Time (s)" class="gt_row gt_right">12.4</td>
<td headers="Total Time (m:s)" class="gt_row gt_right">2:15.7</td></tr>
    <tr><td headers="Sectional Distance (m)" class="gt_row gt_right">2400</td>
<td headers="Sectional Time (s)" class="gt_row gt_right">13.0</td>
<td headers="Total Time (m:s)" class="gt_row gt_right">2:28.7</td></tr>
  </tbody>
  
</table>
</div>

Tap Dance City won this race wire-to-wire by a margin of an incredible
nine lengths. Can you guess how? The sectionals tell the story: Tap
Dance City racked up an enormous lead running at a fairly reasonable
pace, and his rivals — including the formidable Symboli Kris S and the
Double Crown Neo Universe — entirely failed to catch him in the home
stretch.

### Position at Bends: Where was the Winning Horse Relative to its Rivals?

The winner only has to be at the front at the finish line, after all.

In most races, the horses jockey for position near the start, settle
into their position till the final straight, and are then taken “off the
bridle” and ridden hard to the end. As a result, where the racehorse was
at each turn of the racecourse usefully approximates its overall
position.

Take a girl like Gentildonna:

<div id="flozpirmfo" style="padding-left:0px;padding-right:0px;padding-top:10px;padding-bottom:10px;overflow-x:auto;overflow-y:auto;width:auto;height:auto;">
<style>#flozpirmfo table {
  font-family: system-ui, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol', 'Noto Color Emoji';
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

#flozpirmfo thead, #flozpirmfo tbody, #flozpirmfo tfoot, #flozpirmfo tr, #flozpirmfo td, #flozpirmfo th {
  border-style: none;
}

#flozpirmfo p {
  margin: 0;
  padding: 0;
}

#flozpirmfo .gt_table {
  display: table;
  border-collapse: collapse;
  line-height: normal;
  margin-left: auto;
  margin-right: auto;
  color: #333333;
  font-size: 16px;
  font-weight: normal;
  font-style: normal;
  background-color: #FFFFFF;
  width: auto;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #A8A8A8;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #A8A8A8;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
}

#flozpirmfo .gt_caption {
  padding-top: 4px;
  padding-bottom: 4px;
}

#flozpirmfo .gt_title {
  color: #333333;
  font-size: 125%;
  font-weight: initial;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-color: #FFFFFF;
  border-bottom-width: 0;
}

#flozpirmfo .gt_subtitle {
  color: #333333;
  font-size: 85%;
  font-weight: initial;
  padding-top: 3px;
  padding-bottom: 5px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-color: #FFFFFF;
  border-top-width: 0;
}

#flozpirmfo .gt_heading {
  background-color: #FFFFFF;
  text-align: center;
  border-bottom-color: #FFFFFF;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#flozpirmfo .gt_bottom_border {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#flozpirmfo .gt_col_headings {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#flozpirmfo .gt_col_heading {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  overflow-x: hidden;
}

#flozpirmfo .gt_column_spanner_outer {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  padding-top: 0;
  padding-bottom: 0;
  padding-left: 4px;
  padding-right: 4px;
}

#flozpirmfo .gt_column_spanner_outer:first-child {
  padding-left: 0;
}

#flozpirmfo .gt_column_spanner_outer:last-child {
  padding-right: 0;
}

#flozpirmfo .gt_column_spanner {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 5px;
  overflow-x: hidden;
  display: inline-block;
  width: 100%;
}

#flozpirmfo .gt_spanner_row {
  border-bottom-style: hidden;
}

#flozpirmfo .gt_group_heading {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  text-align: left;
}

#flozpirmfo .gt_empty_group_heading {
  padding: 0.5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: middle;
}

#flozpirmfo .gt_from_md > :first-child {
  margin-top: 0;
}

#flozpirmfo .gt_from_md > :last-child {
  margin-bottom: 0;
}

#flozpirmfo .gt_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  margin: 10px;
  border-top-style: solid;
  border-top-width: 1px;
  border-top-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  overflow-x: hidden;
}

#flozpirmfo .gt_stub {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
}

#flozpirmfo .gt_stub_row_group {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
  vertical-align: top;
}

#flozpirmfo .gt_row_group_first td {
  border-top-width: 2px;
}

#flozpirmfo .gt_row_group_first th {
  border-top-width: 2px;
}

#flozpirmfo .gt_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#flozpirmfo .gt_first_summary_row {
  border-top-style: solid;
  border-top-color: #D3D3D3;
}

#flozpirmfo .gt_first_summary_row.thick {
  border-top-width: 2px;
}

#flozpirmfo .gt_last_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#flozpirmfo .gt_grand_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#flozpirmfo .gt_first_grand_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: double;
  border-top-width: 6px;
  border-top-color: #D3D3D3;
}

#flozpirmfo .gt_last_grand_summary_row_top {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: double;
  border-bottom-width: 6px;
  border-bottom-color: #D3D3D3;
}

#flozpirmfo .gt_striped {
  background-color: rgba(128, 128, 128, 0.05);
}

#flozpirmfo .gt_table_body {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#flozpirmfo .gt_footnotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#flozpirmfo .gt_footnote {
  margin: 0px;
  font-size: 90%;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}

#flozpirmfo .gt_sourcenotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#flozpirmfo .gt_sourcenote {
  font-size: 90%;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}

#flozpirmfo .gt_left {
  text-align: left;
}

#flozpirmfo .gt_center {
  text-align: center;
}

#flozpirmfo .gt_right {
  text-align: right;
  font-variant-numeric: tabular-nums;
}

#flozpirmfo .gt_font_normal {
  font-weight: normal;
}

#flozpirmfo .gt_font_bold {
  font-weight: bold;
}

#flozpirmfo .gt_font_italic {
  font-style: italic;
}

#flozpirmfo .gt_super {
  font-size: 65%;
}

#flozpirmfo .gt_footnote_marks {
  font-size: 75%;
  vertical-align: 0.4em;
  position: initial;
}

#flozpirmfo .gt_asterisk {
  font-size: 100%;
  vertical-align: 0;
}

#flozpirmfo .gt_indent_1 {
  text-indent: 5px;
}

#flozpirmfo .gt_indent_2 {
  text-indent: 10px;
}

#flozpirmfo .gt_indent_3 {
  text-indent: 15px;
}

#flozpirmfo .gt_indent_4 {
  text-indent: 20px;
}

#flozpirmfo .gt_indent_5 {
  text-indent: 25px;
}

#flozpirmfo .katex-display {
  display: inline-flex !important;
  margin-bottom: 0.75em !important;
}

#flozpirmfo div.Reactable > div.rt-table > div.rt-thead > div.rt-tr.rt-tr-group-header > div.rt-th-group:after {
  height: 0px !important;
}
</style>
<table class="gt_table" data-quarto-disable-processing="false" data-quarto-bootstrap="false">
  <thead>
    <tr class="gt_heading">
      <td colspan="4" class="gt_heading gt_title gt_font_normal" style>Positional Analysis of Gentildonna</td>
    </tr>
    <tr class="gt_heading">
      <td colspan="4" class="gt_heading gt_subtitle gt_font_normal gt_bottom_border" style>G1 Races Only</td>
    </tr>
    <tr class="gt_col_headings">
      <th class="gt_col_heading gt_columns_bottom_border gt_left" rowspan="1" colspan="1" scope="col" id="Race">Race</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Year">Year</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Pos.-at-Bends">Pos. at Bends</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Finishing-Position">Finishing Position</th>
    </tr>
  </thead>
  <tbody class="gt_table_body">
    <tr><td headers="Race" class="gt_row gt_left">OKA SHO</td>
<td headers="Year" class="gt_row gt_right">2012</td>
<td headers="Pos. at Bends" class="gt_row gt_right">10-10</td>
<td headers="Finishing Position" class="gt_row gt_right">1</td></tr>
    <tr><td headers="Race" class="gt_row gt_left">JAPANESE OAKS</td>
<td headers="Year" class="gt_row gt_right">2012</td>
<td headers="Pos. at Bends" class="gt_row gt_right">13-14-14-15</td>
<td headers="Finishing Position" class="gt_row gt_right">1</td></tr>
    <tr><td headers="Race" class="gt_row gt_left">SHUKA SHO</td>
<td headers="Year" class="gt_row gt_right">2012</td>
<td headers="Pos. at Bends" class="gt_row gt_right">8-9-9-9</td>
<td headers="Finishing Position" class="gt_row gt_right">1</td></tr>
    <tr><td headers="Race" class="gt_row gt_left">JAPAN CUP</td>
<td headers="Year" class="gt_row gt_right">2012</td>
<td headers="Pos. at Bends" class="gt_row gt_right">2-2-3-6</td>
<td headers="Finishing Position" class="gt_row gt_right">1</td></tr>
    <tr><td headers="Race" class="gt_row gt_left">TAKARAZUKA KINEN</td>
<td headers="Year" class="gt_row gt_right">2013</td>
<td headers="Pos. at Bends" class="gt_row gt_right">3-3-3-3</td>
<td headers="Finishing Position" class="gt_row gt_right">3</td></tr>
    <tr><td headers="Race" class="gt_row gt_left">TENNO SHO (AUTUMN)</td>
<td headers="Year" class="gt_row gt_right">2013</td>
<td headers="Pos. at Bends" class="gt_row gt_right">2-2-2</td>
<td headers="Finishing Position" class="gt_row gt_right">2</td></tr>
    <tr><td headers="Race" class="gt_row gt_left">JAPAN CUP</td>
<td headers="Year" class="gt_row gt_right">2013</td>
<td headers="Pos. at Bends" class="gt_row gt_right">3-3-3-4</td>
<td headers="Finishing Position" class="gt_row gt_right">1</td></tr>
    <tr><td headers="Race" class="gt_row gt_left">TAKARAZUKA KINEN</td>
<td headers="Year" class="gt_row gt_right">2014</td>
<td headers="Pos. at Bends" class="gt_row gt_right">4-5-6-6</td>
<td headers="Finishing Position" class="gt_row gt_right">9</td></tr>
    <tr><td headers="Race" class="gt_row gt_left">TENNO SHO (AUTUMN)</td>
<td headers="Year" class="gt_row gt_right">2014</td>
<td headers="Pos. at Bends" class="gt_row gt_right">3-3-3</td>
<td headers="Finishing Position" class="gt_row gt_right">2</td></tr>
    <tr><td headers="Race" class="gt_row gt_left">JAPAN CUP</td>
<td headers="Year" class="gt_row gt_right">2014</td>
<td headers="Pos. at Bends" class="gt_row gt_right">7-7-6-5</td>
<td headers="Finishing Position" class="gt_row gt_right">4</td></tr>
    <tr><td headers="Race" class="gt_row gt_left">ARIMA KINEN</td>
<td headers="Year" class="gt_row gt_right">2014</td>
<td headers="Pos. at Bends" class="gt_row gt_right">3-3-3-2</td>
<td headers="Finishing Position" class="gt_row gt_right">1</td></tr>
  </tbody>
  
</table>
</div>

In most of her G1 efforts, she was raced close to the front, though she
could also win racing from the back. Notice how stable her position at
each bend is. It seems fair enough to say that she was kept in third
position for the 2013 Takarazuka, or held in about ninth place for the
Shuka Sho. This single statistic comprising four numbers is fairly
representative of the flow of her races.

Now consider Gold Ship, who — agent of chaos that he is — illustrates
some of the limitations of this method.

<div id="ittwjcnked" style="padding-left:0px;padding-right:0px;padding-top:10px;padding-bottom:10px;overflow-x:auto;overflow-y:auto;width:auto;height:auto;">
<style>#ittwjcnked table {
  font-family: system-ui, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol', 'Noto Color Emoji';
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

#ittwjcnked thead, #ittwjcnked tbody, #ittwjcnked tfoot, #ittwjcnked tr, #ittwjcnked td, #ittwjcnked th {
  border-style: none;
}

#ittwjcnked p {
  margin: 0;
  padding: 0;
}

#ittwjcnked .gt_table {
  display: table;
  border-collapse: collapse;
  line-height: normal;
  margin-left: auto;
  margin-right: auto;
  color: #333333;
  font-size: 16px;
  font-weight: normal;
  font-style: normal;
  background-color: #FFFFFF;
  width: auto;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #A8A8A8;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #A8A8A8;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
}

#ittwjcnked .gt_caption {
  padding-top: 4px;
  padding-bottom: 4px;
}

#ittwjcnked .gt_title {
  color: #333333;
  font-size: 125%;
  font-weight: initial;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-color: #FFFFFF;
  border-bottom-width: 0;
}

#ittwjcnked .gt_subtitle {
  color: #333333;
  font-size: 85%;
  font-weight: initial;
  padding-top: 3px;
  padding-bottom: 5px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-color: #FFFFFF;
  border-top-width: 0;
}

#ittwjcnked .gt_heading {
  background-color: #FFFFFF;
  text-align: center;
  border-bottom-color: #FFFFFF;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#ittwjcnked .gt_bottom_border {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#ittwjcnked .gt_col_headings {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#ittwjcnked .gt_col_heading {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  overflow-x: hidden;
}

#ittwjcnked .gt_column_spanner_outer {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  padding-top: 0;
  padding-bottom: 0;
  padding-left: 4px;
  padding-right: 4px;
}

#ittwjcnked .gt_column_spanner_outer:first-child {
  padding-left: 0;
}

#ittwjcnked .gt_column_spanner_outer:last-child {
  padding-right: 0;
}

#ittwjcnked .gt_column_spanner {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 5px;
  overflow-x: hidden;
  display: inline-block;
  width: 100%;
}

#ittwjcnked .gt_spanner_row {
  border-bottom-style: hidden;
}

#ittwjcnked .gt_group_heading {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  text-align: left;
}

#ittwjcnked .gt_empty_group_heading {
  padding: 0.5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: middle;
}

#ittwjcnked .gt_from_md > :first-child {
  margin-top: 0;
}

#ittwjcnked .gt_from_md > :last-child {
  margin-bottom: 0;
}

#ittwjcnked .gt_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  margin: 10px;
  border-top-style: solid;
  border-top-width: 1px;
  border-top-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  overflow-x: hidden;
}

#ittwjcnked .gt_stub {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
}

#ittwjcnked .gt_stub_row_group {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
  vertical-align: top;
}

#ittwjcnked .gt_row_group_first td {
  border-top-width: 2px;
}

#ittwjcnked .gt_row_group_first th {
  border-top-width: 2px;
}

#ittwjcnked .gt_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#ittwjcnked .gt_first_summary_row {
  border-top-style: solid;
  border-top-color: #D3D3D3;
}

#ittwjcnked .gt_first_summary_row.thick {
  border-top-width: 2px;
}

#ittwjcnked .gt_last_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#ittwjcnked .gt_grand_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#ittwjcnked .gt_first_grand_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: double;
  border-top-width: 6px;
  border-top-color: #D3D3D3;
}

#ittwjcnked .gt_last_grand_summary_row_top {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: double;
  border-bottom-width: 6px;
  border-bottom-color: #D3D3D3;
}

#ittwjcnked .gt_striped {
  background-color: rgba(128, 128, 128, 0.05);
}

#ittwjcnked .gt_table_body {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#ittwjcnked .gt_footnotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#ittwjcnked .gt_footnote {
  margin: 0px;
  font-size: 90%;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}

#ittwjcnked .gt_sourcenotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#ittwjcnked .gt_sourcenote {
  font-size: 90%;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}

#ittwjcnked .gt_left {
  text-align: left;
}

#ittwjcnked .gt_center {
  text-align: center;
}

#ittwjcnked .gt_right {
  text-align: right;
  font-variant-numeric: tabular-nums;
}

#ittwjcnked .gt_font_normal {
  font-weight: normal;
}

#ittwjcnked .gt_font_bold {
  font-weight: bold;
}

#ittwjcnked .gt_font_italic {
  font-style: italic;
}

#ittwjcnked .gt_super {
  font-size: 65%;
}

#ittwjcnked .gt_footnote_marks {
  font-size: 75%;
  vertical-align: 0.4em;
  position: initial;
}

#ittwjcnked .gt_asterisk {
  font-size: 100%;
  vertical-align: 0;
}

#ittwjcnked .gt_indent_1 {
  text-indent: 5px;
}

#ittwjcnked .gt_indent_2 {
  text-indent: 10px;
}

#ittwjcnked .gt_indent_3 {
  text-indent: 15px;
}

#ittwjcnked .gt_indent_4 {
  text-indent: 20px;
}

#ittwjcnked .gt_indent_5 {
  text-indent: 25px;
}

#ittwjcnked .katex-display {
  display: inline-flex !important;
  margin-bottom: 0.75em !important;
}

#ittwjcnked div.Reactable > div.rt-table > div.rt-thead > div.rt-tr.rt-tr-group-header > div.rt-th-group:after {
  height: 0px !important;
}
</style>
<table class="gt_table" data-quarto-disable-processing="false" data-quarto-bootstrap="false">
  <thead>
    <tr class="gt_heading">
      <td colspan="4" class="gt_heading gt_title gt_font_normal" style>Positional Analysis of Gold Ship</td>
    </tr>
    <tr class="gt_heading">
      <td colspan="4" class="gt_heading gt_subtitle gt_font_normal gt_bottom_border" style>G1 Races Only</td>
    </tr>
    <tr class="gt_col_headings">
      <th class="gt_col_heading gt_columns_bottom_border gt_left" rowspan="1" colspan="1" scope="col" id="Race">Race</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Year">Year</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Pos.-at-Bends">Pos. at Bends</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Finishing-Position">Finishing Position</th>
    </tr>
  </thead>
  <tbody class="gt_table_body">
    <tr><td headers="Race" class="gt_row gt_left">SATSUKI SHO</td>
<td headers="Year" class="gt_row gt_right">2012</td>
<td headers="Pos. at Bends" class="gt_row gt_right">18-18-17-6</td>
<td headers="Finishing Position" class="gt_row gt_right">1</td></tr>
    <tr><td headers="Race" class="gt_row gt_left">TOKYO YUSHUN (JAPANESE DERBY)</td>
<td headers="Year" class="gt_row gt_right">2012</td>
<td headers="Pos. at Bends" class="gt_row gt_right">13-13-11-10</td>
<td headers="Finishing Position" class="gt_row gt_right">5</td></tr>
    <tr><td headers="Race" class="gt_row gt_left">KIKUKA SHO</td>
<td headers="Year" class="gt_row gt_right">2012</td>
<td headers="Pos. at Bends" class="gt_row gt_right">17-17-4-2</td>
<td headers="Finishing Position" class="gt_row gt_right">1</td></tr>
    <tr><td headers="Race" class="gt_row gt_left">ARIMA KINEN</td>
<td headers="Year" class="gt_row gt_right">2012</td>
<td headers="Pos. at Bends" class="gt_row gt_right">16-15-14-10</td>
<td headers="Finishing Position" class="gt_row gt_right">1</td></tr>
    <tr><td headers="Race" class="gt_row gt_left">TENNO SHO (SPRING)</td>
<td headers="Year" class="gt_row gt_right">2013</td>
<td headers="Pos. at Bends" class="gt_row gt_right">14-13-6-4</td>
<td headers="Finishing Position" class="gt_row gt_right">5</td></tr>
    <tr><td headers="Race" class="gt_row gt_left">TAKARAZUKA KINEN</td>
<td headers="Year" class="gt_row gt_right">2013</td>
<td headers="Pos. at Bends" class="gt_row gt_right">4-4-3-4</td>
<td headers="Finishing Position" class="gt_row gt_right">1</td></tr>
    <tr><td headers="Race" class="gt_row gt_left">JAPAN CUP</td>
<td headers="Year" class="gt_row gt_right">2013</td>
<td headers="Pos. at Bends" class="gt_row gt_right">16-17-13-13</td>
<td headers="Finishing Position" class="gt_row gt_right">15</td></tr>
    <tr><td headers="Race" class="gt_row gt_left">ARIMA KINEN</td>
<td headers="Year" class="gt_row gt_right">2013</td>
<td headers="Pos. at Bends" class="gt_row gt_right">12-11-8-4</td>
<td headers="Finishing Position" class="gt_row gt_right">3</td></tr>
    <tr><td headers="Race" class="gt_row gt_left">TENNO SHO (SPRING)</td>
<td headers="Year" class="gt_row gt_right">2014</td>
<td headers="Pos. at Bends" class="gt_row gt_right">18-18-15-14</td>
<td headers="Finishing Position" class="gt_row gt_right">7</td></tr>
    <tr><td headers="Race" class="gt_row gt_left">TAKARAZUKA KINEN</td>
<td headers="Year" class="gt_row gt_right">2014</td>
<td headers="Pos. at Bends" class="gt_row gt_right">4-3-4-4</td>
<td headers="Finishing Position" class="gt_row gt_right">1</td></tr>
    <tr><td headers="Race" class="gt_row gt_left">ARIMA KINEN</td>
<td headers="Year" class="gt_row gt_right">2014</td>
<td headers="Pos. at Bends" class="gt_row gt_right">11-10-6-5</td>
<td headers="Finishing Position" class="gt_row gt_right">3</td></tr>
    <tr><td headers="Race" class="gt_row gt_left">TENNO SHO (SPRING)</td>
<td headers="Year" class="gt_row gt_right">2015</td>
<td headers="Pos. at Bends" class="gt_row gt_right">14-14-3-4</td>
<td headers="Finishing Position" class="gt_row gt_right">1</td></tr>
    <tr><td headers="Race" class="gt_row gt_left">TAKARAZUKA KINEN</td>
<td headers="Year" class="gt_row gt_right">2015</td>
<td headers="Pos. at Bends" class="gt_row gt_right">16-16-14-15</td>
<td headers="Finishing Position" class="gt_row gt_right">15</td></tr>
    <tr><td headers="Race" class="gt_row gt_left">JAPAN CUP</td>
<td headers="Year" class="gt_row gt_right">2015</td>
<td headers="Pos. at Bends" class="gt_row gt_right">17-17-15-5</td>
<td headers="Finishing Position" class="gt_row gt_right">10</td></tr>
    <tr><td headers="Race" class="gt_row gt_left">ARIMA KINEN</td>
<td headers="Year" class="gt_row gt_right">2015</td>
<td headers="Pos. at Bends" class="gt_row gt_right">16-16-2-3</td>
<td headers="Finishing Position" class="gt_row gt_right">8</td></tr>
  </tbody>
  
</table>
</div>

Of course, Gold Ship also had a fairly consistent strategy. He did not
go from last to first in the final straight. Rather, he was raced behind
for the first half or so of the race; then he would unleash a very long
spurt and overtake most of his rivals before even hitting the final
turn. (The Takarazukas are notable exceptions.) In such a case, it is
difficult to capture his positioning with a single number: in his final
Arima, was he raced in the 16th position, or in 2nd, or do we go
halfsies, take the average, and say that 9th place represents his
positioning best?

In the end, I decided to use *median* position at bends as the single
number that best represents a horse’s overall positioning. 18-18-17-6
becomes 17.5; 16-16-2-3 becomes 9.5. This is an unsatisfactory solution,
to be sure. The only consolation is that these cases are not very
common.\*

There are other caveats to this statistic. 2-2-2-2 can represent two
completely different situations: a horse who’s leading the pack far
behind the front runner, or a horse that’s matching the front runner’s
pace stride for stride. Moreover, if the racers are grouped tightly,
going from 16th place to 1st in the home straight might look more
impressive on paper than in practice. This complexity is not captured —
and cannot be captured — with just a single number.

Interpret responsibly!

### Does the Early Pace Dictate the Winner’s Positioning?

To recapitulate, received wisdom has it that a fast early pace makes
life easier for the late surgers, while a slow early pace favours those
stalking at the front. Moreover, Tokyo Racecourse is reputed to favour
backliners. If so, we *should* find that winners of the Japanese Derby
are likelier to come from behind if the early sectionals are fast.

I chose the time taken to run 600m as my metric for “early pace”, and
plotted it with the median position at bends for each of the Derby
winners. My dataset extends back to 1993, and I included only Derbies
that were run on ground rated “Good”. I have included a least-squares
regression line for illustrative purposes — *not* to demonstrate
correlation or statistical significance!

![](https://github.com/WishfullyThinking/wishfullythinking.github.io/images/derby-graph-1.png)

The connection here seems very weak. Fast Derbies have been won by
horses towards the front; slow Derbies have been won by those running at
the back.

How about the other three-year-old Fuchu G1, the NHK Mile? We’ll look at
both the 600m and the 400m sectionals, because it’s a shorter race.

![](https://github.com/WishfullyThinking/wishfullythinking.github.io/images/nhk-mile-graph-1.png)![](https://github.com/WishfullyThinking/wishfullythinking.github.io/images/nhk-mile-graph-2.png)

Intriguingly, the general pattern *does* seem to hold true for the NHK
Mile, in a way that it doesn’t for the Japanese Derby.

What happens if we look at *podium* finishes, not just the winners?

![](https://github.com/WishfullyThinking/wishfullythinking.github.io/images/podium-graph-1.png)![](https://github.com/WishfullyThinking/wishfullythinking.github.io/images/podium-graph-2.png)

Interestingly, this seems to barely shift the picture. In fact, the top
3 *within the same year* seem to come from all over the place, too, and
in no particular order.
