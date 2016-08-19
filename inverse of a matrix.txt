nrow=5; ncol=5
values=sample(1:(nrow*ncol), (nrow*ncol))
makeCacheMatrix <- function(x = matrix(values,nrow,ncol)) { 
    #set initial value of matrix inverse
    invMTX <- NULL
    
    #check if number of rows is equal to number of columns
    if(nrow==ncol){ #test to determine the nrow=ncol
        invMTX <<- solve(x)  #cache for inverse of matrix
    } else {
        print ("number of rows must be equal to number of columns") #return the result of the comparison
    }
    
    
}
cacheSolve <- function (x = matrix(values,nrow,ncol)){
    invMTX <- x #establish the cache
    #check if equality between nr of rows and nr of columns  has a zero value
    if (!is.null(nrow==ncol)) {
        message ("getting cached data") 
        return(x)
    }
}

makeCacheMatrix
matrix(values,nrow,ncol)
solve(makeCacheMatrix)
