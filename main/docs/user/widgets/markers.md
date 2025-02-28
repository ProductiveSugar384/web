---
sidebar_position: 6
title:  Marker widgets
---

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';
import AndroidStore from '@site/src/components/buttons/AndroidStore.mdx';
import AppleStore from '@site/src/components/buttons/AppleStore.mdx';
import LinksTelegram from '@site/src/components/_linksTelegram.mdx';
import LinksSocial from '@site/src/components/_linksSocialNetworks.mdx';
import Translate from '@site/src/components/Translate.js';
import InfoIncompleteArticle from '@site/src/components/_infoIncompleteArticle.mdx';

## Overview

Map markers are selected points marked with flags on the map. They provide useful information for navigating to direct points on the map screen.

## Top bar widget (markers)  


<Tabs groupId="operating-systems">

<TabItem value="android" label="Android">  

![Map markers on the Top bar widget](@site/static/img/widgets/map_markers_top_bar_widget.png)

</TabItem>

<TabItem value="ios" label="iOS">  

![Map markers on the Top bar widget](@site/static/img/widgets/map_markers_top_bar_widget_ios.png)

</TabItem>

</Tabs> 

On the top bar widget you could see the distance and the direction to the marker from current location. It is possible to configure to see 1 or 2 top markers in the widget.

| | |
|------------|------------|
| Enable | <Translate android="true" ids="shared_string_menu,map_markers_item"/>→ ≡ →<Translate android="true" ids="appearance_on_the_map,shared_string_topbar"/> |
| On Click | Centers map view to the marker position |
| On Map Hold | In order to measure the distance and view the direction from a specific map point to the map marker, press & hold on the map and slightly change map position (so context menu won't open) |
| Approach marker | In case your location is within a short radius of the map marker (< 50m), you could see a quick button to remove the map marker (mark as passed).  |
| Format distance | **<Translate android="true" ids="android_button_seq"/>:** <Translate android="true" ids="shared_string_menu,configure_profile,general_settings_2,units_and_formats,unit_of_length"/>  |
|        | **<Translate ios="true" ids="ios_button_seq"/>:**  <Translate ios="true" ids="menu,sett_settings,app_profiles,general_settings_2,units_and_formats,unit_of_length"/> |


## Panel widgets (markers)  

<Tabs groupId="operating-systems">

<TabItem value="android" label="Android">  

![Panel widgets](@site/static/img/widgets/map_markers_widget.png) ![Panel widgets](@site/static/img/widgets/map_markers_widget_settings.png)

On panel widgets **"Distance"** and **"Estimated time of arrival"** to the map marker are displayed.

:::note
**"Estimated time of arrival" (ETA)** is the value that is calculated as the distance to the marker / the average speed. 

_The average speed_ is calculated from a specified interval (15sec - 60 min). For example, we have 300 location points with speed data during a specified 10 min. Average speed is the sum of speeds from points data / 300.

_The distance to the marker_ is a straight distance from your position (or a specific map point) to the marker.
:::

| | |
|------------|------------|
| Enable | <Translate android="true" ids="shared_string_menu,map_markers_item"/>→ ≡ →<Translate android="true" ids="appearance_on_the_map,shared_string_widgets"/>  |
|  | <Translate android="true" ids="shared_string_menu,map_widget_config,shared_string_widgets"/> |
| On long tap | Centers map view to the marker position |
| On short tap | Changing between "Distance" / "Estimated time of arrival" |
| On Map Hold | In order to measure the distance and view the direction from a specific map point to the map marker, press & hold on the map and slightly change map position (so context menu won't open) |
| Format | **<Translate android="true" ids="android_button_seq"/>:** <Translate android="true" ids="shared_string_menu,configure_profile,general_settings_2,units_and_formats,unit_of_length"/> |


</TabItem>

<TabItem value="ios" label="iOS">  

![Panel widgets](@site/static/img/widgets/map_markers_widget_ios.png)

On panel widgets only distance to the map marker is displayed.

| | |
|------------|------------|
| Enable | <Translate android="true" ids="shared_string_menu,map_markers_item"/>→ ≡ →<Translate android="true" ids="appearance_on_the_map,shared_string_widgets"/>  |
| On Click | Centers map view to the marker position |
| On Map Hold | In order to measure the distance and view the direction from a specific map point to the map marker, press & hold on the map and slightly change map position (so context menu won't open) |
| Format | **<Translate ios="true" ids="ios_button_seq"/>:**  <Translate ios="true" ids="menu,sett_settings,app_profiles,general_settings_2,units_and_formats,unit_of_length"/>  |


</TabItem>

</Tabs> 


## Configure Marker widgets and Marker appearance

All marker appearance settings and widget parameters are configured through the same menu.

<Tabs groupId="operating-systems">

<TabItem value="android" label="Android">  

**<Translate android="true" ids="android_button_seq"/>:** <Translate android="true" ids="shared_string_menu,map_markers_item,appearance_on_the_map"/> 

![appearence_on_the_map](@site/static/img/widgets/appearence_on_the_map.png)


</TabItem>

<TabItem value="ios" label="iOS">  

**<Translate ios="true" ids="ios_button_seq"/>:**  <Translate ios="true" ids="menu,map_markers,appearance_on_map"/> 

![Map markers Appearance iOS](@site/static/img/personal/markers/map_markers_appearance_ios.png) 


</TabItem>

</Tabs> 

|    | Description    | State | 
| :------------- | :------------- | :------------- |
| <Translate android="true" ids="active_markers"/> | Specifies a number of direction indicators| 1 or 2 | 
|  <Translate android="true" ids="show_direction"/> | Specifies how direction indicators should be displayed | <Translate android="true" ids="shared_string_topbar"/> / <Translate android="true" ids="shared_string_widgets"/>| 
|  <Translate android="true" ids="show_arrows_on_the_map"/> |  Displays arrows on the map to the top markers in case they are not part of the visible map | - |
| <Translate android="true" ids="show_guide_line"/> | Shows direction line from user location to the top markers  | - |
| <Translate android="true" ids="one_tap_active"/> (**Android**) |  Displays / switches marker in the widget by tapping on a marker on the map. |  - | 
| <Translate android="true" ids="keep_passed_markers"/> (**Android**) | Keeps or hides inactive markers on the map, if a marker is part of the visible group of Favorites or GPX waypoints. | -  |
