# The Evolution of Space Missions
# Global Overview
Purposes: Give executives or viewers a high-level snapshot of all missions and their outcomes.

# Executive Summary
# 1. Mission Growth Over Time
- The dataset spans 1957 - 2022, covering the entire modern space age.
- Two major surges:
  1. 1960s-1980s: Driven by the US-USSR space race.
  2. 2000s-2020s: driven by private sector growth (SpaceX, CASC, Ariancespace).
  3. Modern launches are more commercialized and frequent, reflecting llower costs, and reusable rockets.

# 2. Market Share by Organization
- Top 5 operators (RVSN USSR, CASC, Arianespace, General Dynamics, VKS RF) account for ~60% of all missions.
- Indicated state-dominated launches historically, but with commercial entrants growing after 2000.

# 3. Mission Reliability
| Status            | Count | %     |
| ----------------- | ----- | ----- |
| Success           | 4,162 | 89.8% |
| Failure           | 357   | 7.7%  |
| Partial Failure   | 107   | 2.3%  |
| Prelaunch Failure | 4     | 0.1%  |

- Reliability > 89% shows maturity of space tech
- Failures cluster in early decades (1950s - 1970s)

# 4. Launch Economics
| Status              | Avg. Launch Price (M USD) |
| ------------------- | ------------------------- |
| Retired Rockets     | 258.4                     |
| Active Rockets      | 68.6                      |
| Successful Missions | 131.2                     |
| Failed Missions     | 55.5                      |

- Older (retired) rockets were costlier and less efficient.
- Modern active rockets are most cost-effective and reusable.
- Higher cost correlates with success, suggesting better hardware or mission preparedness.

# Methodology
Dataset Overview
Rows: 4632
Columns: 9
Columns Names: Company Name, Location, Date, Time, Rocket, Mission, Rocket Status, Mission Status

# Data Cleaning
| Metric                 | Result                  |
| ---------------------- | ----------------------- |
| **Date range**         | 1957-03-11 → 2022-12-07 |
| **Non-missing prices** | 1,265 out of 4,632 rows |
| **Min price**          | $2.5 million            |
| **Max price**          | $5,000 million          |
| **Mean price**         | $128.3 million          |

The dataset is now cleaned with:
- Consistent column names (lowercase, underscores)
- Dates parsed to datetime
- Prices numeric and ready for aggregation

# Exploratory Data Analysis
<img width="1231" height="604" alt="image" src="https://github.com/user-attachments/assets/88920294-7065-4b74-931e-ce14a34a38f2" />

Missions Over Time
- Space missions span from 1957 - 2022
- Strong early growth in the 1960s-1980s (space race era);
- Noticeable acceleration again post-2000 due to private companies like SpaceX and CASC.

<img width="1083" height="618" alt="image" src="https://github.com/user-attachments/assets/15aaebcd-d838-4ca8-a035-e5dc8af9e249" />

Top Companies by Number of Missions
| Rank | Company                   | Missions |
| ---- | ------------------------- | -------- |
| 1    | **RVSN USSR**             | 1,777    |
| 2    | **CASC (China)**          | 338      |
| 3    | **Arianespace (France)**  | 293      |
| 4    | **General Dynamics (US)** | 251      |
| 5    | **VKS RF (Russia)**       | 216      |

The dataset is dominated by government and military programs, with commercial launches increasing in later years.

<img width="669" height="609" alt="image" src="https://github.com/user-attachments/assets/cc55ec97-f018-4455-8786-14fb089bfb72" />

Mission Success Rate
| Status                | Count | %     |
| --------------------- | ----- | ----- |
| **Success**           | 4,162 | 89.8% |
| **Failure**           | 357   | 7.7%  |
| **Partial Failure**   | 107   | 2.3%  |
| **Prelaunch Failure** | 4     | 0.1%  |

Almost 90% of missions were successful.

<img width="1008" height="607" alt="image" src="https://github.com/user-attachments/assets/34a99421-03fb-447f-9484-9e39f75112a4" />

Average Launch Price By Rocket Status
| Rocket Status | Avg. Price (Million USD) |
| ------------- | ------------------------ |
| **Retired**   | 258.4                    |
| **Active**    | 68.6                     |

Retired rockets tend to higher historical costs - likely due to older technologies or less efficient designs.

<img width="1008" height="608" alt="image" src="https://github.com/user-attachments/assets/0bbf2064-1a9a-4a5b-8e58-188dff1632d6" />

Average Launch Price By Mission Status
| Mission Status        | Avg. Price (Million USD) |
| --------------------- | ------------------------ |
| **Success**           | 131.2                    |
| **Partial Failure**   | 131.2                    |
| **Prelaunch Failure** | 62.0                     |
| **Failure**           | 55.5                     |

Successful missions generally have higher launch costs - possibly refelcting better technology, more advanced rockets, or higher-value payloads.

<img width="1004" height="609" alt="image" src="https://github.com/user-attachments/assets/dce18016-e018-4158-ab42-6785a2d0093b" />

Top 10 Countries by Number of Missions
| Rank | Country              | Missions |
| ---- | -------------------- | -------- |
| 1    | 🇺🇸 **USA**         | 1,467    |
| 2    | 🇷🇺 **Russia**      | 1,416    |
| 3    | 🇰🇿 **Kazakhstan**  | 719      |
| 4    | 🇨🇳 **China**       | 365      |
| 5    | 🇫🇷 **France**      | 318      |
| 6    | 🇯🇵 **Japan**       | 130      |
| 7    | 🇮🇳 **India**       | 82       |
| 8    | 🌊 **Pacific Ocean** | 36       |
| 9    | 🇳🇿 **New Zealand** | 28       |
| 10   | 🇮🇷 **Iran**        | 16       |

The USA and Russia dominate launch activity - accounting for over 60% of all missions.

# Recommendations
- Invest in modern, active rockets.
- Titl volume toward USA/Russia for capacity, grow share with China/India for cost & diversification.
- Smooth demand with multi-year planning.





