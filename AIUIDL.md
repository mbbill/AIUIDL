
# Elements:
Elements are represented as JSON objects.
Each element must have a unique 'id' and a 'type' (e.g., 'button', 'text', 'container', etc.).
Properties can be added to customize appearance and behavior.

## Inheritance:
Child elements do not inherit properties from their parents by default.
Inheritance can be implemented in the custom renderer if desired.

# Nesting:
Elements can be nested using a 'children' property, an array of elements.
Allows for complex UI scenarios, including nested layouts and components.

# Layout:
AIUIDL supports 'flex', 'grid', and 'stack' layout methods.
Common layout properties include:
For 'flex': 'direction', 'alignItems', 'justifyContent', 'flexWrap', 'flexGrow', 'flexShrink', 'flexBasis', 'order'.
For 'grid': 'gridTemplateColumns', 'gridTemplateRows', 'gridGap', 'gridColumn', 'gridRow', 'gridColumnStart', 'gridRowStart', 'gridColumnEnd', 'gridRowEnd'.
For 'stack': 'stackDirection', 'stackSpacing', 'stackAlignment', 'stackJustify'.

# Styles:
Styles are JSON objects applied to elements via a 'style' property.
Common style properties include:
Positioning: 'position', 'top', 'right', 'bottom', 'left', 'zIndex'.
Box Model: 'width', 'height', 'padding', 'paddingTop', 'paddingRight', 'paddingBottom', 'paddingLeft', 'margin', 'marginTop', 'marginRight', 'marginBottom', 'marginLeft', 'border', 'borderTop', 'borderRight', 'borderBottom', 'borderLeft', 'borderRadius', 'boxSizing'.
Typography: 'fontFamily', 'fontSize', 'fontWeight', 'fontStyle', 'textDecoration', 'textAlign', 'lineHeight', 'color', 'letterSpacing', 'textTransform', 'whiteSpace', 'wordWrap', 'textOverflow'.
Background: 'background', 'backgroundColor', 'backgroundImage', 'backgroundSize', 'backgroundPosition', 'backgroundRepeat', 'backgroundAttachment'.
Display: 'display', 'visibility', 'opacity', 'overflow', 'overflowX', 'overflowY'.
Animation: 'transition', 'transform', 'animation', 'animationDuration', 'animationTimingFunction', 'animationDelay', 'animationIterationCount', 'animationDirection', 'animationFillMode', 'animationPlayState'.

# Events:
Event handlers can be added using 'on[EventName]' properties (e.g., 'onClick').
Values should be function names, implemented in the custom renderer.
Event dispatching is determined by the custom renderer.
Event bubbling (propagation) behavior should be implemented in the custom renderer if desired.

# Custom Components:
Define custom components with a unique 'type' and required properties.
Components should be implemented in the custom renderer.
