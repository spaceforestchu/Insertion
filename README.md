# Insertion

        function insert(arr){
        var key, j;
            for( j = 1; j < arr.length; j++){
                 key = arr[j];
               var i = j - 1;
                while(i >= 0 && arr[i] > key){
        
                    arr[i+1] = arr[i];
                    i = i - 1;
                }
                arr[i + 1] = key;
            }
          return arr;
        }
        
        insert([5, 2, 4, 6, 1, 3,69,25,4]);
