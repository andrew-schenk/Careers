# Technical 1
## DBA/Backend

There are two short questions.  That's right, you get to have twice the fun as the frontend developer.  :sunglasses:

### Question 1
Given these tables

gatekeeper_user | &nbsp; | &nbsp;
--------------- | - | -
id (primary key) | email (varchar) | belongs_to_circle_id (fk)

common_circles | &nbsp;
-------------- | - 
id (primary key) | name (varchar)


Write a MYSQL (5.7 compatible) query that fetches all unique email domains and counts them for circle name 'Retailer'.  Email data should be considered valid format.  e.g. 'john@example.com'

Expected Result format

domain | count
------ | ------
acme.com | 5
example.com | 10

---

### Question 2
You receive this pull request from a colleague.  They are wanting to add a `CreateEvent` API endpoint to the Python/Django app.  Do you approve or deny this code?  If you deny it, what comments if any would you provide to your colleague?

```python
class CreateEvent(TemplateView):
    def get(self, request, *args, **kwargs):
        return self.process(request, *args, **kwargs)

    def post(self, request, *args, **kwargs):
        return self.process(request, *args, **kwargs)

    def process(self, request, *args, **kwargs):

        try:
            if request.user.groups.first().name == "Viewer"
                return JsonResponse(
                    {'error': true, "message": 'Your account is not permitted to creat events'})
        except:
            return JsonResponse({'error': True, 'message': 'You have to be logged in to create events'})

        try;
            newEvent = Event.objects.create(created_by_user=request.user)
            newEvent.save()
        except:
        return JsonResponse({'error': True, 'msg': 'There was an error creating the event'});

        return JsonResponse(
            {'error': false, 'message': 'The event has been created successfully', 'data': {'event_id': new_event.id}})
```


Create a gist for your answers and email the link to careers@linxsystems.com
