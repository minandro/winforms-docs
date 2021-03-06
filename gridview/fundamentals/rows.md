---
title: Rows
page_title: Rows | UI for WinForms Documentation
description: Rows
slug: winforms/gridview/fundamentals/rows
tags: rows
published: True
position: 5
previous_url: gridview-fundamentals-rows
---

# Rows

There are two main row types in RadGridView: 

* Data rows

* Structure rows

## DataRows

Each data row in the grid represents a record from the specified __DataSource__. Each __RadGridView__ has a row collection of type [GridViewRowInfo]({%slug winforms/gridview/rows/gridviewrowinfo%}). The collection provides methods to add or remove items.
      	

>note Note that only Rows bound to the data source are kept in the Rows collection. The header, pager, filter and separator are not included in this collection.

__Selected row__

You can check if a grid row is in selected state using __GridRowElement.IsSelected__ property. Multiple rows can be selected if the RadGridView __MultiSelect__ property is set to *True*.
![gridview-fundamentals-row 001](images/gridview-fundamentals-row001.png)

## Structure Rows

__FilteringRow__

Filtering row will appear automatically when you have [Filtering]({%slug winforms/gridview/filtering/basic-filtering%}) enabled either by __RadGridView.EnableFiltering__ or __GridViewTemplate.EnableFiltering__ properties.<br>![gridview-fundamentals-overview-of-radgridview-structure 004](images/gridview-fundamentals-overview-of-radgridview-structure004.png)

__HeaderRow__

The header element is represented by __GridHeaderRowElement__ object.
![gridview-fundamentals-overview-of-radgridview-structure 002](images/gridview-fundamentals-overview-of-radgridview-structure002.png)

__Add New Row__

Depending of the value of the __GridViewTemplate.AddNewRowPosition__ property the new row element appears below the header row or after the data rows.<br />![gridview-fundamentals-overview-of-radgridview-structure 003](images/gridview-fundamentals-overview-of-radgridview-structure003.png)
