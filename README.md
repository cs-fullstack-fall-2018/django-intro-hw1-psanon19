# django-intro-hw1

Create a new route and paste it below. Create a blue-or-red route that takes an argument of blue or red. If it's blue, write "Sky". If it's red, write "Fire". If it's anything else write "ERROR".



path('<userinput>/colors', views.blue_or_red),

def blue_or_red(request, userinput):

        if userinput=="red":

            return HttpResponse(("Got your color: Fire"))

        elif userinput=="blue":

            return HttpResponse(("Got your color: blue"))

        else:

            return HttpResponse(("Error"))


        return HttpResponse(("Got your color"))
