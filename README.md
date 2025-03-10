# ServiceDesignTrial
A Service Design Trial by Rachel A.Wood
# Sample data frame with service design tools and their phases
tools <- data.frame(
  tool = c("Customer Journey Mapping", "Prototyping", "Stakeholder Interviews", "User Testing"),
  phase = c("Develop", "Deliver", "Discover", "Define"),
  stringsAsFactors = FALSE
)

# Print original data frame
print("Original Data:")
print(tools)

# Convert 'phase' column to an ordered factor based on the Double Diamond phases
tools$phase <- factor(tools$phase, levels = c("Discover", "Define", "Develop", "Deliver"))

# Sort the data frame by the 'phase' column
tools_sorted <- tools[order(tools$phase), ]

# Print the sorted data frame
print("Sorted Data by Double Diamond Phases:")
print(tools_sorted)
