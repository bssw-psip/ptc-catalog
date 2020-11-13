# Algorithm Productization Checklist

## Target

A VTK-m filter for ALPINE in situ algorithm users.

## User Story

As an algorithm developer, I want to develop and productize an ECP-relevant algorithm so it is a robust VTK-m filter available to ECP applications through ALPINE infrastructure and running on exascale hardware.   

## Card

| Task | Description |
|:-----:|:------------|
|  0 | A research implementation or definition may exist |
|  1 | A baseline implementation exhibiting correct behavior is committed to a repository such as [ALPINE Algorithm github](https://github.com/Alpine-DAV/algorithms), Kitware GitLab, or lab-specific GitLab |
|  2 | A parallel distributed implementation has been tested on applicable sets of ECP application data with demonstrated utility  |
|  3 | The implementation is ported to VTK-m as a worklet with a wrapping filter |
|  4 | The VTK-m version has been verified on applicable data |
|  5 | Unit tests have been implemented for the filter
|  6 | Pull requests have been created for the VTK-m worklet/filter and nightly CI build is successful |
|  7 | The VTK-m filter has been demonstrated within ALPINE infrastructure using a proxy or an ECP app integration |
|  8 | The VTK-m filter has been demonstrated on an exascale machine or exascale proxy
|  9 | Scaling and performance testing has been completed and documented in relevant P6 Activity Report
| 10 | Documentation (geared towards an application user) is available in [ALPINE Algorithm github](https://github.com/Alpine-DAV/algorithms) |
| 11 | Documentation is available in VTK-m documentation |

## Notes

- Some algorithms may go through a phase with both VTK-h and VTK-m code
- Development of VTK-m filters must adhere to the [VTK-m contributing guide](https://gitlab.kitware.com/vtk/vtk-m/blob/master/CONTRIBUTING.md)
