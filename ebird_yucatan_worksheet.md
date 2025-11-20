
# eBird Yucatan Practical – Worksheet

Name: ___________________________   Date: ________________

This worksheet accompanies the practical session using the
Yucatan Peninsula teaching datasets:

- `ebird_yucatan_checklists.csv`
- `ebird_yucatan.csv`
- `ebird_yucatan_traits.csv`

Answer in bullet points or short paragraphs. Attach key figures if requested.

## Part 0A – Excel exploration exercises

Before using R, explore the datasets in Microsoft Excel (or LibreOffice Calc, Google Sheets).

### Exercise 0A.1: Checklist data

1. How many checklists are in the dataset?

2. What is the date range (earliest to latest observation)?

3. List the land cover categories. Which has the most checklists?

4. What is the typical range of species richness per checklist? (Create a histogram)

5. What is the average effort in hours per checklist?

### Exercise 0A.2: Species detection data

6. How many total species detection records are there?

7. How many unique species are in the dataset?

8. Which species appears in the most checklists? (Use Pivot Table)

9. What is the maximum count recorded for any species in a single checklist?

### Exercise 0A.3: Trait data

10. How many species have trait data available?

11. What are the smallest and largest body masses in the dataset?

12. What trophic niche categories are present?

13. Create a scatter plot of body mass vs wing length. Do you see a relationship?

### Exercise 0A.4: Reflection

14. What are some challenges of working with these data in Excel?

15. What questions would be easier to answer with R?


## Part 0 – First look at the data in R

16. How many checklists are there in the dataset? Compare with your Excel count.

17. Over which years were they collected?

18. Which land cover types are represented?


## Part 1 – Mapping and richness

19. Attach or sketch the map of checklist locations across the Yucatan Peninsula region.
    Which areas appear most heavily sampled?

20. Using species richness per checklist (`n_species`), which land cover type has the highest
    average richness? Which has the lowest?

21. Give one ecological explanation for the observed difference in richness
    between **forest** and **urban** checklists (if present).

### Part 1.3 – Spatial density mapping

22. Where is sampling effort most concentrated in the Yucatan Peninsula based on the 
    kernel density map?

23. How does the distribution of your focal species compare to overall sampling effort?

24. Why might it be important to account for sampling effort when interpreting
    species distribution patterns?

25. Compare the hexagonal binning approach to kernel density estimation. 
    What are the advantages of each method?

26. How do the total count and mean count hexbin maps differ in their interpretation?
    Which is more useful for understanding species distribution?


## Part 2 – Species trends (reporting rates)

27. For selected focal species in the dataset:

    a. Describe how their reporting rates changed over time.  
    b. Which species appears more common or more widely reported?  
    c. Suggest one reason why a species might show a flat trend vs. a strong increase or decrease.

28. Imagine that habitat loss disproportionately affects forest areas.
    How might that influence the real reporting rate of forest-dependent species?


## Part 3 – Communities across land cover types

29. Which species are most frequently detected in **forest** checklists?
    Which dominate **urban** or **agricultural** checklists?

30. Are there any species that occur across all land cover types with high frequency?
    What does that suggest about their ecology?


## Part 4 – Functional diversity

31. Compare the functional richness (FRic) among land cover types:

    a. Which land cover type has the highest FRic?  
    b. Which has the lowest?  
    c. What might this imply about the range of ecological roles in each land cover type?

32. Look at FEve and FDiv for the same land cover types. Choose one land cover type and
    interpret what its combination of FRic, FEve and FDiv tells you about the
    structure of the bird community.

33. According to Matthews et al. (2024), bird extinctions can cause
    disproportionate loss of functional diversity. How might selective loss
    of large-bodied or specialised species alter FRic in a real-world community?


## Part 5 – Traits and habitat filtering

34. Using the body mass histogram by land cover:

    a. Which land cover type tends to have the largest-bodied species?  
    b. Which land cover type is dominated by smaller species?  
    c. Briefly discuss why body size might be associated with sensitivity to
       human disturbance or hunting.

35. How might the preferential loss of large-bodied species affect ecosystem
    processes such as seed dispersal or carrion removal? Give one example.


## Part 6 – Optional: PCA of traits

36. Which traits mainly drive PC1 and PC2 in the trait space?

37. Discuss where species with different trophic niches lie in this trait space.


## Part 7 – Synthesis

38. Summarise, in 5–6 sentences, what your analyses of the teaching dataset
    suggest about:

    - differences in richness among land cover types,  
    - typical species in human-modified vs. less disturbed land cover types, and  
    - how trait structure (functional diversity) changes with land cover.

39. How could citizen-science data such as eBird help conservationists identify
    priority areas or species for protection in the Yucatan Peninsula?

40. Name one limitation of using eBird data for these types of analyses, and
    suggest a way to mitigate it.

41. How do your findings conceptually link to the key messages of Stewart et al. 
    and Matthews et al. about habitat loss and functional diversity loss?

