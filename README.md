## R Assignment ##
## Cache Matric and inverse #

makeCacheMatrix <- function( X = matrix () ) {
inv = NULL
set = function (y) {
X  <<- y
inv << - NULL
}
get = function () X
set inv = function (inverse)   inv <<- inverse
getinv =  function() inv
list (set=set, get=get, setinv=setinv, getinv=getinv)
}

cacheSolve <- function(X, …)  {
inv = X$getinv()
if ( ! is.null (inv))  {
message ( “ cached data “)
return (inv)
}	
mat.data = x$get()
inv =  solve( mat.data, …)
X$setinv (inv)
return (inv)
}

