# testgitHubIntegration

My class1{
private int number = 0;
Private String str;
//add comments one1
//second was added3
}


    steps:
      

        with:
          asana-secret: ${{ secrets.ASANA_SECRET }}
          comment-text: " {{PR_URL}} with id {{PR_ID}} and {{PR_NAME}} name was {{PR_STATE}}."
      - name: Get status
        run: echo "Status is ${{ steps.createComment.outputs.status }}"
