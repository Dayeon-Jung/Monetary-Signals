# Monetary-Signals

### FOMC Statements and U.S. Dollar Movements: Why Do Market Reactions Differ Across Meetings?

## Project Overview

This project examines the relationship between the tone of Federal Open
Market Committee (FOMC) statements and short-term movements in the U.S.
Dollar Index (DXY). In particular, we investigate whether hawkish or
dovish changes in the Federal Reserve's language are associated with
dollar movements around FOMC announcements, and why market reactions
differ across meetings.

Our preliminary analysis shows a weak positive relationship between
changes in statement tone and two-day DXY returns. Some large dollar
movements also occur close to announcement dates. These patterns
motivate further investigation, but they do not establish that FOMC
announcements caused the movements.

## Research Questions

1.  Are DXY movements around FOMC announcements consistent with changes
    in statement tone? What evidence suggests that the movements are
    related to the announcements, and what evidence suggests otherwise?
2.  How do the content and hawkish or dovish tone of FOMC statements
    differ between announcements with large DXY movements and those
    without large movements?
3.  What other economic or financial factors could explain DXY
    movements, especially when statement tone does not explain them
    well?

## Data

The study uses:

-   **FOMC statements:** 47 statements from January 2021 through October
    2026, collected from the Federal Reserve website.
-   **U.S. Dollar Index (DXY):** 1,466 daily closing observations,
    downloaded from Yahoo Finance using Python's `yfinance` package.
-   **Additional variables for analysis:** Treasury yields, the VIX, and
    information about inflation and employment releases.

## Methodology

-   Use Gemini and a scoring guide to assess each FOMC statement's tone
    on a scale from **-1 (strongly dovish)** to **+1 (strongly
    hawkish)**.
-   Calculate changes in statement tone between consecutive FOMC
    meetings.
-   Examine DXY returns on the announcement day and the following
    trading day.
-   Identify extreme movements as returns more than **2.5 standard
    deviations** from the previous **60-trading-day average**.
-   Compare statement content and tone across announcements with large
    DXY movements and those without large movements.
-   Consider other economic and financial factors that may help explain
    movements not captured by statement tone.

## Preliminary Findings

The proof-of-concept analysis compares changes in FOMC statement tone
with combined DXY log returns on the announcement day and the next
trading day for 46 meetings.

The preliminary results show:

-   A weak positive relationship between changes in statement tone and
    two-day DXY returns.
-   Considerable variation in DXY returns, even among meetings with
    similar tone changes.
-   Some large daily DXY movements occurring near FOMC announcement
    dates.

These findings support further comparison of individual announcements
and consideration of other possible explanations. The preliminary graph
does **not** demonstrate that FOMC announcements caused the observed
dollar movements.

## Limitations

-   Statement-tone scores involve subjective judgment.
-   Only 46 usable changes in statement tone are available.
-   Only two announcement windows meet the preliminary definition of
    extreme movements.
-   Other news and economic developments can affect daily DXY returns
    around announcement dates.

For these reasons, the analysis focuses on exploring relationships and
possible explanations rather than claiming causation.

## Data Sources

-   [Federal Reserve](https://www.federalreserve.gov/): FOMC statements
-   [Yahoo Finance](https://finance.yahoo.com/): Daily DXY closing
    values

## Tools

-   Python
-   `yfinance`
-   Gemini-assisted statement-tone scoring
-   Git and GitHub
