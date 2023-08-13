# @c0sm0-kramer
## interests
I am interested in scientific computing
## what languages do I have reasonable proficiency with ?
Fortran 90/95, a good amount of 03, and working towards full utilization of 08
### contact
```fortran
program contact

  implicit none
  character(len=10), parameter   :: domain = "@gmail.com"
  character(len=99)              :: local_part
  character(len=: ), allocatable :: email

  local_part = "fortran90programming"

  allocate ( character( len_trim(local_part) + len(domain) ) :: email )

  email = local_part( 1:len_trim(local_part) ) // domain

  print '(A)', email

  deallocate ( email )

end program contact
```

