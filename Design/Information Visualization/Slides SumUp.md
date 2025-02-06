# 1. **Intro**

## **What?**
### **Visualization Scope**
- **Scientific Visualization (SciVis)**: geometry is given (volumetric data), tackles problems in 3D space; 
- **Geographic Visualization (GeoVis)**: geographic data, tackles geographic phenomena, established and well known techniques; 
- **Information Visualization (InfoVis)**: abstract data, broader purpose, techniques should be created or carefully designed, polished aesthetics; 
- **Visual Analytics (VA)**: DataVis + data mining, focus on the analysis of ML algorithms and outputs.

## **Why?**
- Graphs are an extremely important means for communicating quantitative information. Graphs are used extensively to convey information because they do so effectively;
- Quantitative patterns and relationships in data are easily revealed by graphs because of the enormous power the cognitive-visual system to perceive geometrical patterns;
- This system can summarise vast amounts of quantitative information on a graph, perceiving distinctive features, or focusing on specific details.

Overcome limits:
- Human: Cognition and Memory; 
- Computer: Processing time and System memory; 
- Display: Display size and pixel density / space used to encode information: information density.

## **Static vs Dynamic Visualizations**
### **Static**
Static visualizations present information in a fixed format, emphasizing clarity and organization to communicate a specific message effectively.
Focus:
- Order
- Message
Goal: Communication
### **Dynamic**
Dynamic visualizations allow users to interact with the data, enabling deeper analysis and exploration through adjustable parameters and real-time feedback.
Focus:
- Interaction
Goal: Analysis and Exploration

## **Expressiveness vs. Effectiveness**
### **Expressiveness**
- **Explanation**: A visualization is expressive when it encodes all relevant information while excluding unnecessary details, ensuring a concentrated and precise representation of data.
- **Measure**: The concentration of information.
### **Effectiveness**
- **Explanation**: A visualization is effective when it presents information clearly and efficiently, minimizing effort and time to achieve understanding.
- **Measure**: The cost of achieving information awareness.

---
# 2. **Visualization Process**

## **Steps**
1. Define the problem and target users;
2. Translation (Abstraction)
	- Data Abstraction
	- Task Abstraction
3. Design visual encodings and interactions
4. Implementation
5. Validation

## **Translation**
Translate the problems and data from the vocabulary of the domain into an abstract description that is in the vocabulary of information visualization.
### **Data Abstraction**
#### **Data Types**
- **Tables**: Data arranged in rows and columns.
- **Networks**: Data represented as interconnected nodes and edges.
- **Spatial**:
    - **Fields**: Continuous data distributed across a space (e.g., temperature maps).
    - **Geometry**: Data representing shapes, positions, or spatial structures.
#### **Attribute Types**
- **Categorical**: Qualitative data without inherent order (e.g., colors, names).
- **Ordered**: Data with inherent order:
    - **Ordinal**: Ranked data without precise differences (e.g., ratings: low, medium, high).
    - **Quantitative**: Numeric data with measurable differences (e.g., temperature, age).
#### **Ordering**
- **Sequential**: Ordered progression (e.g., low to high).
- **Diverging**: Data diverging around a central neutral point (e.g., profit vs. loss).
- **Cyclic**: Data with repeating patterns (e.g., months, hours of the day).

### **Task Abstraction**
Task abstraction focuses on understanding the purpose and objectives of a visualization by addressing key questions:
- **Why is the user using visualization?**  
    To gain insights, understand patterns, or communicate information effectively.
- **What questions do you want to answer?**  
    Define specific inquiries or problems the visualization should clarify.
- **What problem are you trying to solve?**  
    Identify the challenge or knowledge gap the visualization aims to address.
- **What decision are you trying to make?**  
    Determine how the visualization will support decision-making or strategy.
- **What outcomes are you hoping for?**  
    Clarify desired results, such as better understanding, persuasive storytelling, or improved analytics.
- **What story do you want to tell?**  
    Highlight the narrative or key message the visualization conveys to the audience.
- **What tasks should the viewer be able to perform?**  
    Specify interactive or analytical tasks, such as filtering, comparing, or exploring data.

## **Design Visual Encodings and Interactions**
### Key Concepts:
1. **Arrangement**:
    - Refers to spatial organization, layout, and expressiveness of visual elements.
    - It's about how visual components are structured to convey the data effectively.
2. **Mapping**:
    - The process of translating data types into visual marks and their properties (visual variables or channels).
### Supporting Principles:
- **Semiology of Graphics**:
    - The study of how visual symbols represent data.
- **Visual Information Perception**:
    - Understanding how humans interpret visual information for effective communication.
- **Gestalt Principles**:
    - Perception laws that describe how viewers group visual elements (e.g., proximity, similarity).
### **Visual Channels (Properties):**
- **Position**: Where elements are located on a plane.
- **Size**: Relative or absolute size differences in elements.
- **Value**: Lightness or darkness to represent data.
- **Texture**: Patterns or fills for differentiation.
- **Color**: Hue and saturation to indicate distinctions.
- **Orientation**: Direction or angle of elements.
- **Shape**: Form of elements (e.g., circle, square).

Each channel can be:
- **Associative**: Helps group similar elements.
- **Selective**: Distinguishes elements from others.
- **Order**: Implies a sense of ranking or sequence.
- **Quantitative**: Encodes measurable differences.

# Data Design

![[Pasted image 20250123171606.png]]

## **Bar Chart**
![[Pasted image 20250123171737.png]]
- **Data Types**:
    - Works best with **discrete** data categories.
    - Can be used to represent **temporal data** for trends or comparisons.
- **Purpose**:
    - Primarily used for **comparison** between categories or across time.
- **Design Features**:
    - **Size proportional to value**: The length or height of bars reflects the magnitude of the data.
    - **Horizontal labels**: Categories should be clearly labeled below the bars for readability.
    - **Y-axis starts at 0**: Ensures accurate perception of proportional differences.
    - **Ordered**: Bars should be arranged logically, either by value (descending/ascending) or as per categorical or temporal order.

## **Line Chart** 
![[Pasted image 20250123171956.png]]
- **Data Types**:
    - Best suited for **continuous data**, especially over time (**temporal data**).
- **Purpose**:
    - Used to identify **patterns and trends** over a continuous range (e.g., time, measurements).
- **Design Guidelines**:
    - **No more than 5 lines**: Avoid clutter to ensure readability and focus on key comparisons.
    - **Include 0 on scale (if possible)**: Helps provide context and prevent misleading interpretations.
    - **Aspect ratio**: Aim for an average slope of **45 degrees** to balance visual clarity and the perceived steepness of changes.

## **Area Chart**
![[Pasted image 20250123172121.png]]
- **Data Types**:
    - Ideal for **continuous data**, particularly across a timeline (**temporal data**).
- **Purpose**:
    - Used for **comparison** of cumulative values or to show proportions over time.
- **Design Guidelines**:
    - **Sort areas**: Stack areas logically, either by importance or magnitude, to avoid confusion.
    - **Y-axis starts at 0**: Ensures accurate representation of the data magnitude.
    - **Use transparency**: Apply transparency to overlapping areas to maintain visibility and clarity.

## **Bubble Chart**
![[Pasted image 20250123172206.png]]
- **Data Types:**
    - **Nominal data**: Ideal for displaying categories without order.
    - **Comparison**: Allows comparison of data points across categories.
    - **Ranking**: Bubble size can represent magnitude or rank, helping identify larger or more significant categories.
- **Purpose:** Bubble charts are used to show relationships between categories, comparing multiple variables by representing their magnitude with bubble size.
- **Design Guidelines:**
    - **Use area, not radius**: Represent size by area for proportional accuracy.
    - **Use transparency**: Apply transparency to overlapping bubbles for better clarity.
    - **Sort logically**: Group or position bubbles by importance or magnitude.
    - **Ensure contrast**: Make sure bubbles stand out from the background and each other.
    - **Limit bubbles**: Too many can clutter the chart—use them sparingly for clarity.


## **Pie Chart**
![[Pasted image 20250123172740.png]]
- **Data Types:**
    - **Partitional data**: Pie charts represent parts of a whole, with each segment showing a specific category’s contribution.
    - **Comparison**: They allow comparisons between different segments, highlighting proportions of the total.
- **Purpose:** Pie charts are used to show how different categories make up a whole. The size of each slice is proportional to its percentage of the total (100%).
- **Design Guidelines:**
    - **Proportional area**: Each segment’s area should directly correspond to its proportion of the total circle.
    - **No more than 5 slices**: Limit the number of slices to avoid overcrowding the chart, ensuring readability.
    - **Sort in clockwise direction**: Arrange the slices starting from the top left, moving clockwise, for consistency and ease of interpretation.
    - **Sum must be 100%**: The total of all slices must add up to 100% to represent the whole accurately.
    - **Use contrasting colors**: Differentiate slices clearly with contrasting colors to improve readability.

## **Scatterplot**
![[Pasted image 20250123173127.png]]
- **Data Types:**
    - **High-density data**: Scatterplots are ideal for displaying large sets of data points to identify trends or patterns.
    - **Correlation and patterns**: Used to explore the relationship between two variables, showing how they correlate or form patterns.
- **Purpose:** Scatterplots visually represent individual data points within a coordinate system, helping to reveal trends, correlations, and patterns in the data.
- **Design Guidelines:**
    - **Y-axis starts at 0**: Always start the Y-axis at 0 to maintain accuracy and avoid distorting the data.
    - **Use trend lines**: Add trend lines to highlight patterns or relationships between the variables.
    - **Focus on data density**: Scatterplots are effective for high-density data, helping to identify patterns amidst large numbers of points.
    - **Ensure clarity**: Space the points adequately and consider transparency for overlapping data points to avoid visual clutter.

## **Heat Map**
![[Pasted image 20250123173223.png]]
- **Data Types:**
    - **Nominal & Ordinal data**: Heat maps are useful for displaying categorical data (nominal) and ordered categories (ordinal), such as rankings or ratings.
    - **Comparison**: They are effective for comparing values across different categories or variables.
    - **Ranking**: Heat maps can show rankings or relative intensity across categories.
- **Purpose:** Heat maps are used to visually represent data in matrix format, with color intensity indicating the magnitude of values, making it easy to compare and identify trends or patterns.
- **Design Guidelines:**
    - **Simple outline**: Keep the structure of the heat map clean with clear gridlines or boundaries for better readability.
    - **Single color with varying shades**: Use one color with different shades to represent varying levels of intensity, ensuring clarity and consistency.
    - **Avoid multiple patterns**: Stick to color intensity rather than adding patterns or textures, as this could create visual confusion and reduce effectiveness.

---

# 3. **Data Preprocessing**

## 1. **Gather/Select**
Different types of data sources: 
- Surveys – interviews using a set of predefined questions; 
- Experiments – measure and collect data in a highly controlled manner; • Observational – large number of observations are taken; 
- Data warehouses – a copy of data taken from different sources that has been cleaned, normalised, and optimised; 
- Purchased databases – data taken from different source and combined with the in house datasets

## 2. **Discover and Categorize**
### **Discover**
Know the data and understand what has to be done before the data becomes useful in a particular context. • What to search for? • • • • What are the question(s) to solve (or prove wrong)? What kind of data it is and how to treat different types? What is missing from the data and how to deal with it? Where are the outliers and how should they be cared about?

### **Categorize**
- Know the data types with which you will work with; 
- Data types: continuous vs discrete; 
- Scales of measurement: Nominal, Ordinal, Interval, and Ratio; 
- Visualize the frequency distribution with: 
	- Dot plot
	- Histograms

## 3. **Clean and Validate**
- **Validity**: Check data-type constraints and range constraints, set-membership constraints, and regular expression patterns; 
- **Accuracy**: The degree to which the data is close to the true values. 
- **Completeness**: The degree to which all required data is known. 
- **Consistency**: The degree to which the data is consistent, within the same data set or across multiple data sets. 
- **Uniformity**: The degree to which the data is specified using the same unit of measure

Measures Examples:
- Spell Check
- Range Check
- Removing Unnecessary Data

## 4. **Transform the data**
Consist in application of mathematical transformations to the data in order to make it compatible with other data or graphical elements. 
Data transformation can also reveal hidden information that is not observable in the original form. 
Some common transformations: 
- **Scaling Values**
- **Reduce Skewness** 
- **Value mapping** 
- **Discretization** 
- **Aggregation**

### **Scaling Values**
Process in which numeric variables are transformed into a new range;
The common normalization methods are: 
- Min-max
- Z-score
- Decimal scaling

#### **Min-Max**
Transform the variable to a new range.
![[Pasted image 20250123192655.png]]

### **Reduce Skewness**
If the variable does not conform normal distribution, consider application of the following transforms:

| Method      | Math            | Good                                                                                | Bad                                              |
| ----------- | --------------- | ----------------------------------------------------------------------------------- | ------------------------------------------------ |
| Log         | ln(x), log₁₀(x) | Right-skewed data; log₁₀(x) is great for handling powers of 10 (e.g., 1000, 100000) | Zero values, Negative values                     |
| Square root | sqrt(x)         | Right-skewed data                                                                   | Negative values                                  |
| Square      | x²              | Left-skewed data                                                                    | Negative values                                  |
| Cube root   | x^(1/3)         | Right-skewed data, Negative values                                                  | Less effective at normalizing than log transform |
| Reciprocal  | 1/x             | Makes small values bigger and big values smaller                                    | Zero values, Negative values                     |

With the logarithmic we can highlight the smaller values and analyze its evolution, whether in the linear it is not possible to have that detail.
![[Pasted image 20250123193045.png]]

### **Value Mapping**
Many methods require the values to be in numeric form; 
In cases of discrete data the values might be replaced with numbers. 
Example: 
- {low, medium, high} -> {0, 1, 2}

### **Discretization**
Convert continuous data into discrete values; 
This type of conversation sometimes called binning; 
Examples: 
- Credit score can be mapped to {poor, average, good, excellent} 
- Weight {<40, 40-50, 50-60, >60}


