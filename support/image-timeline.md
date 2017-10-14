# Image Timeline - Support

Power BI custom visual by David Eldersveld  

### Contact me on ![Twitter](https://twitter.com/dataveld) @dataveld   
### Log an Issue on ![GitHub](https://github.com/deldersveld/pbiImageTimeline/issues)  

The Image Timeline is a custom visual for Microsoft Power BI that displays events along a horizontal timeline. Events appear as either circles or custom images.  

![](https://raw.githubusercontent.com/deldersveld/pbiImageTimeline/master/assets/timeline.PNG)  

![](https://raw.githubusercontent.com/deldersveld/pbiImageTimeline/master/assets/timeline-no-image.PNG)

![](https://raw.githubusercontent.com/deldersveld/pbiImageTimeline/master/assets/timeline-measure-resizes.PNG)

## Functionality  
- *Date brush* - Interactively adjust the date range using the "brush" at the top of the visual. Drag the left side of the brush to alter the start date and the right side to alter the end date. Once you have a smaller range, you can also drag the center of the brush to move along the timeline.
![](https://raw.githubusercontent.com/deldersveld/pbiImageTimeline/master/assets/timeline-brush.PNG)  
- *Images* or *Points*- Add optional images using URLs in your dataset. If an Image URL is not specified, timeline events appear as points.

## Fields
The Image Timeline has options for four fields:  
![](https://raw.githubusercontent.com/deldersveld/pbiImageTimeline/master/assets/fields.PNG)  
- *Category* - A required column containing individual events.
- *Sequence/Date* - A column that spreads events along the timeline. By default, the visual displays the timeline based on the minimum and maximum dates/datetimes from this field.
- *Image URL* - An optional column that provides images to display for each event. URL values in the dataset must start with HTTP or HTTPS. If no Image URL is supplied for this field, timeline events display as points. 
- *Measure* - An optional measure / numeric field that appears on tooltips and can also be used to resize events (if desired).

## Format Options  
There are several format options available to customize the timeline:  

![](https://raw.githubusercontent.com/deldersveld/pbiImageTimeline/master/assets/format-options.PNG)  
- *Brush base color* - Alter the color of the date brush at the top of the visual.
- *Event color* - Alter the color of timeline events if images are not used (currently one color for all events).
- *Date display* - Select how date labels appear in the brush and on tooltips.
- *Measure resizes image* - Enable or disable the ability for measure values to resize images or timeline events. Higher measure values equal larger points or images.
- *Require HTTPS image links* - Force image links to contain HTTPS. If an Image URL starts with HTTP and not HTTPS, timeline events will display as points and not images even when the Image URL field is otherwise a valid image.


## Version History  
### 1.1.0 - Initial public release
- Interactive date brush
- Timeline events as points or images


## License  
The Image Timeline for Power BI is licensed under the MIT License.
