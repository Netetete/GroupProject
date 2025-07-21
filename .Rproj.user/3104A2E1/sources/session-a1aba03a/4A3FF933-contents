#Starting this for when we need it

# install.packages("arrow")
# install.packages("tidyverse")
library(arrow)
library(tidyverse)
library(sf)


df <- read_parquet("merged_data.parquet")

# converting tabular parquet to geo parquet
df <- st_as_sf(df)

# Export to shapefile
st_write(df, "spatial_merged_data.shp")
