# NTPU-Programming-for-Data-Science

# .personalInfo
.personalInfo <- list(
  name="danma",
  id="410973013",
  gmail="dan40410@gmail.com"
)

.date=lubridate::today()
.newRmd <- paste0(.date,".Rmd")
.skeletonRmd <- readLines("https://raw.githubusercontent.com/tpemartin/econDS/master/inst/rmarkdown/templates/inclass-practice/skeleton/skeleton.Rmd")
if(!file.exists(.newRmd)){
  purrr::map_chr(
    .skeletonRmd, ~{glue::glue(.x, .open="<<", .close=">>")}
  ) -> .myRmd
  writeLines(.myRmd, con=.newRmd)
}
