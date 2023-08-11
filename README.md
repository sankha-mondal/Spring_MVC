# Spring MVC :
Spring MVC is a framework for building web applications in Java. As the name suggests, it's based on the Model-View-Controller design pattern.

# Core Components of Spring MVC :
⚪ DispatcherServlet:
	◼ Spring's Front Controller implementation

⚪ Controller :
	1. User created component for handling requests                                                                                            
 	2. Encapsulates navigation logic
  	3. Delegates to the service objects for business logic
   	4. The default handler is a very simple Controller interface with the method:
		ModelAndView handleRequest(request, response).

⚪ View :
	1. Responsible for rendering output

⚪ ModelAndView :
	1. Created by the Controller
	2. Stores the Model data
	3. Associates a View to the request
		◻ Can be a physical View implementation or a logical View name
	4. The ModelAndView class is simply a container by which the model may be transported to and exposed by the view.
		It is not the model itself

⚪ ViewResolver :
	1. Used to map logical View names to actual View implementations

⚪ HandlerMapping :
	1. Strategy interface used by DispatcherServlet
	2. for mapping incoming requests to individual Controllers 
