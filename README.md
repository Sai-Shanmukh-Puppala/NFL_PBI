# NFL Player Performance Dashboard

## Overview
This repository contains a PowerBI dashboard designed to analyze NFL player performance. The dashboard leverages a star schema design, focusing on key metrics that provide insights into player performance across different positions. Our goal was to create a streamlined and user-friendly tool that can be used by analysts, fans, and other stakeholders interested in NFL statistics.

## Star Schema Implementation
The dataset is structured using a star schema, which simplifies querying and enhances the performance of the PowerBI report. The star schema consists of the following components:

- **Fact Table (`PlayerStats`)**: Contains the performance metrics for each player, including statistics like passing yards, rushing touchdowns, sacks, and more.
- **Dimension Tables**:
  - **Players**: Information about the players, including player names, positions, and team associations.
  - **Teams**: Contains the team names and corresponding team IDs, along with URLs for the team logos.
  - **Opponents**: Contains the opponent team names and corresponding team IDs, along with URLs for the team logos.
  - **Dates**: Includes information about the season and week, allowing for time-based analysis.
  - **player_stats**: Consists of game-wise player stats.

## Key Features
- **Position-Specific Metrics**: The dashboard dynamically displays metrics relevant to the selected player's position. For example, when viewing a quarterback, you'll see metrics like passing yards and touchdowns.
- **Dynamic Titles**: The titles of metrics displayed in the dashboard update automatically based on the selected player's position group, ensuring clarity and relevance.
- **Team Logo Integration**: Each player’s performance is visually associated with their team through dynamically loaded team logos, which also serve as the background for visuals.
- **Interactive Slicers**: Users can filter the dashboard by player, season, and week to drill down into specific timeframes and player performances.

## How to Use
1. **Download the Repository**: Clone or download this repository to your local machine.
2. **Open in PowerBI Desktop**: Load the `NFL Player Performance.pbix` file into PowerBI Desktop.
3. **Interact with the Dashboard**: Use the slicers to filter by player and season, and observe the dynamic updates in the metrics and visuals.
