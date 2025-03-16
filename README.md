# Marketing Mix Modeling (MMM) Data Analysis Dashboard

## Project Overview
The **Marketing Mix Modeling (MMM) Data Analysis Dashboard** is an object-oriented programming project that analyzes marketing campaign performance using statistical and machine learning techniques. The system enables businesses to quantify the impact of various marketing activities on sales and key performance indicators (KPIs), helping optimize future marketing strategies.

## Team Members
- **Abdel Raouf Lakhoues**
- **Becher Zribi**
- **El Amine Maaloul**
- **Omar Allal**
- **Yassine Marrekchi**

## Features
### 1. **Choice of Data**
- Supports `.csv` and `.xlsx` file formats for input.
- Users select the dataset to be analyzed.

### 2. **Overview of Data**
- Displays a summary of the dataset, including structure, types, and basic statistics.
- Provides an interface for data exploration before further analysis.

### 3. **Statistical & Correlation Analysis**
- Computes essential statistical metrics.
- Generates a **Correlation Matrix** to identify relationships between variables and detect multicollinearity issues.

### 4. **Visualizations & Exploratory Data Analysis (EDA)**
- **Pie Chart:** Displays expenditure distribution across different marketing channels.
- **Line Chart:** Tracks sales trends across various campaigns to highlight peak and underperforming periods.

### 5. **Sales Prediction**
- Implements a **Decision Tree Model** to predict future sales.
- Uses input features from the dataset and provides predicted sales values.

## Object-Oriented Programming (OOP) Principles
### 1. **Inheritance: Code Reusability & Extensibility**
- `DataSource.java`: Defines a generic data source structure.
- `CSVReader.java` & `XLSXReader.java`: Extend `DataSource` and implement format-specific reading logic.
- `MachineLearningModel.java`: Interface defining `train` and `predict` methods.
- `Model.java`: Implements the interface with machine learning logic.

### 2. **Polymorphism: Flexible Behavior Implementation**
- `Visualization.java`: Contains methods to create different chart types (`createPieChart`, `createLineChart`).
- `displayChart()` method adapts dynamically to different visualization types, improving flexibility.

### 3. **Encapsulation: Data Security & Controlled Access**
- `Model.java`: Restricts direct access to `decisionTree`, `trainingInstances`, and `attributeList` using `private` variables.
- `DataPreprocessor.java`: `removeDuplicates()` is private to enforce data integrity.

### 4. **Abstraction: Simplified System Design**
- `MachineLearningModel.java`: Defines an abstract structure without exposing implementation details.
- `Dashboard.java`: Abstracts UI generation through modular methods (`createChartsPanel()`, `createPredictionPanel()`).

## Setup & Installation
### Prerequisites
- **Java Development Kit (JDK)** 8 or later.
- **Apache POI** (for `.xlsx` file processing).
- **JFreeChart** (for data visualization).

### Installation Steps
1. Clone the repository:
   ```sh
   git clone https://github.com/your-repo/MMM-Data-Analysis.git
   ```
2. Navigate to the project folder:
   ```sh
   cd MMM-Data-Analysis
   ```
3. Compile the Java files:
   ```sh
   javac -cp ".:lib/*" src/*.java
   ```
4. Run the application:
   ```sh
   java -cp ".:lib/*" src.Main
   ```

## Usage Guide
1. Run the application and upload a `.csv` or `.xlsx` file.
2. Explore the **Overview Tab** for dataset insights.
3. Navigate to **Statistical Analysis** to inspect correlations.
4. Check **Charts Tab** for visual trends in marketing spend and sales.
5. Visit **Predictions Tab** to forecast sales using the decision tree model.

## Future Enhancements
- Implement additional machine learning models (e.g., Random Forest, XGBoost).
- Expand visualization options (e.g., heatmaps, histograms).
- Add user authentication and session management.
- Optimize UI for a more interactive dashboard experience.

## License
This project is licensed under the **MIT License**.

## Contact
For inquiries or contributions, please contact:
- Becher Zribi - [Your Email or LinkedIn]
- GitHub Repository: [Your GitHub Repo Link]

---
**Marketing Mix Modeling Dashboard - 2025**
