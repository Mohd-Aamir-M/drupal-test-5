# Test for Drupal 8

## Task 1 - Create a Content Type for Hospitals with following detail:

1. Name
2. Address
3. Phone number
4. Speciality (taxonomy) -> One hospital can have multiple speciality like "Cariology", "Neurology", "Opthamology" etc.
5. picture

## Task 2 - Create a customer role which will be used by Mobile app users to simply register with their name and email.

## Task 3 - Create a API using Rest API Module using Views Rest Export:

1. User registration (API should register user as a customer and role should be assigned to him)
2. User login
3. Get Content of Hospital (retrive all content of hospital)

Note: the request format should be very normalize that means easy for frontend developer to read the content. Consider the example with couple of hospital response and expected response.

[
{
nodeId: 100,
name: 'ABC hospital',
phone: '999999999',
picture: 'url-of-picture.jpg'
speciality : [
        {
          'targe_id':1,
          'cardiology'
        },
        {
          'targe_id':2,
          'Neurology'
        }
       ]
},
{
nodeId: 100,
name: 'XYZ hospital',
phone: '989898989',
picture: 'url-of-picture.jpg'
speciality : [
        {
          'targe_id':1,
          'cardiology'
        },
        {
          'targe_id':2,
          'gynocology'
        },
                {
          'targe_id':3,
          'pediatric'
        }
       ]
}
]


