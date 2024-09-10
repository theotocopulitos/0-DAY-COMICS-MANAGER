# 0-DAY-COMICS-MANAGER
A script to help identify and sort comics from 0-day packs, and tag them using comicvine

My use case: getting 0-day packs and then passing them over either to comicrack or to komga requires a lot of work in terms of sorting and tagging. This script (WIP) is aimed at reducing the overhead derived from this process. To do so, it does the following:

1. **Get a 0-day list**:

     Now it gets the list from comicvine, using the 0-day pack name to determine the release date to look for. CV 0-day lists are far from complete, but on a first approach, it is the most convenient way to proceed, since this way we get the CV ID for each 0-day comic. I'd like to get a more complete 0-week elsewhere and match the comics in that list to this CV ID, but that should be a future version. So far, I am sticking to the convenience over completeness.

2. **Match comics in the folder against those in the list**:

    I am trying a loose matching strategy... let's see how that works

3. **Tag and move matched comics**:

     Comics successfully matched will be tagged with essential info (CV ID, Series, number and little more), and moved to a subdirectory named after the series, so Komga can work with them. Having the CV ID there helps for detailed scrapping by other tools (ComicRack, Komga, etc...). Sometime along the road, I can implement complete scraping and tagging.

    The folders for each comic will get an ID like a series.json file or the like (got to check what CR, and Komga offer or need).
   
