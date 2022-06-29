## Welcome to my Home

### Example
##### Update many documents

The same way I was able to update one document with `updateOne()`, I can update multiple documents with `updateMany()`.

    filter = eq("student_id", 10001);
    updateResult = gradesCollection.updateMany(filter, updateOperation);
    System.out.println("\n=> Updating all the documents with {\"student_id\":10001}.");
    System.out.println(updateResult);


In this example, I'm using the same `updateOperation` as earlier, so I'm creating a new one element array `comments` in these 10 documents.

Here is the output:

    => Updating all the documents with {"student_id":10001}.

AcknowledgedUpdateResult{matchedCount=10, modifiedCount=10, upsertedId=null}

##### The findOneAndUpdate method

Finally, we have one last very useful method available in the MongoDB Java Driver: `findOneAndUpdate()`.

> In most web application, when a user update something, he wants to see
> this update reflected in his web page. Without the
> `findOneAndUpdate()` method, you would have to run an update operation
> and then fetch the document with a find operation to make sure you are
> printing the latest version of this object in the web page.

The `findOneAndUpdate()` method allow you to combine these two operations in one.

<div align=center>
<img src="readme_md_files/6cd843b0-f78b-11ec-8ce8-a964dda655a4.jpeg?v=1&type=image" width = "300" height = "300" alt="图片名称"/>
<p>KissesJun</p></div>

## FAQ
### Why my Twitter account is locked?
> **Standard Application**
> 
> I just didn't use my account for a long time, I didn't reach any rules, and I couldn't receive confirm codes and calls too, on my phone when I wanna resolve the secure problem by verifying my phone number.

- [ ] Edit at 2022-6-29 17:11:46
