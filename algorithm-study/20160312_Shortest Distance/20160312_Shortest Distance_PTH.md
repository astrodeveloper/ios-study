```Swift
import UIKit

func getShortestDistance(array: [Int]) -> (Int, Int) {
  let index = zip(array, array[1..<array.count]).map{$0.1 - $0.0}.sort(<).first!
  return (array[index], array[index + 1])
}

var array = [1, 3, 4, 8, 13, 17, 20]

print(getShortestDistance(array))
```
 
