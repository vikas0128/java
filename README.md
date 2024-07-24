// lexicographical order in the array by the selection sort


    static void selection_sort_question(String []arr)
    {
       for(int i=0;i<arr.length;i++)
       {
           int min=i;

           for(int j=i+1;j< arr.length;j++) {
               if (arr[j].compareTo(arr[min])<0) {
                   min = j;
               }
           }
           String swap=arr[i];
           arr[i]=arr[min];
           arr[min]=swap;

       }

    }
    public static void main(String[] args)
    {


        String[] arr={"vikas","arple","rajat","arb an","banana"};
        selection_sort_question(arr);

        for (int i = 0; i < arr.length; i++) {
            String ar = arr[i];
            System.out.println(ar);
        }




    }


}
