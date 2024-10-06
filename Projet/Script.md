# Script

## Slide 1

- Now we proceed onto the Methodology section

## Slide 2

- The methodology section is mainly a technical description of what was done to take into consideration 3 primary concerns:
  - First, the extent to which the normalization is affected by the lesion definition
  - Second, as the source image is smoothed before normalization, another concern lies in determining the optimal cost function mask expansion as in "which near areas will be affected by the lesion the smoothing"
  - Third, the procedures to make a qualitative assessment of the quality of the proposed normalization technique as compared to the de facto normalization (affine only)

## Slide 3

- Regarding the used database, we have:
  - 10 TI MRI images of brains with lesions
  - 4 set of observers (3 of which were residents and one of which was an experienced psychologist)
  - The SPM99 software was used to some preliminary pre-processing, to define default parameters for the normalization, but most importantly to define 2 template masks:
    - The template brain mask which is derived from the mean of many MRI of healthy brains
    - The thresholded template brain mask, which is a mask to exclude areas outside of the brain
  - We also have 10 simulated lesion images, for which it was necessary 10 MRIs of healthy brains and the mask of the
    - To create the simulated lesion images what was done was the following:
      - Project the voxels of the damaged and the healthy brain on the template
      - Use the parameters determined by the lasts normalizations to project the damaged brain on the voxel space of the healthy brain
      - Use the same parameters to project the mask (lesion definition from set 1)
      - Calculate the scale factor
        - Calculate the masked means (area inside the brain, but outside the area of lesion) of both the normal brain and the damaged brain
      - Calculate the simulated lesion image
- We can now compare the normalization of the simulated lesion images and the normal brain using the root mean square of deformation fields (the Euclidean norm of the difference of the dislocations)

## Slide 4

- Moving on to the lesion area expansion
- The authors created many processed normalization masks which were done in the following way:
  - smooth the lesion definitions from sets 2..4
  - invert resulting image
  - and finally threshold the image
- On the right side we can see the many thresholds that were used as well as their corresponding expansion
- Finally with the procedure I talked about on the previous slide we can compare 5 normalizations and the standard normalization of the healthy brain image

## Slide 5

- Proceeding on to the qualitative assessment
  - The authors compared the affine plus non linear normalization with a processed mask and that of affine only normalization
- In this context, the authors measured:
  - Similarity between normalized images
  - Similarity of normalized images to the template
