# Spring MVC :
Spring MVC is a framework for building web applications in Java. As the name suggests, it's based on the Model-View-Controller design pattern.

# Core Components of Spring MVC :
⚪ DispatcherServlet:
	- Spring's Front Controller implementation

⚪ Controller:
	- User created component for handling requests
	- Encapsulates navigation logic
	- Delegates to the service objects for business logic
	- The default handler is a very simple Controller interface with method:
		ModelAndView handleRequest(request, response).

⚪ View:
	- Responsible for rendering output

⚪ ModelAndView:
	- Created by the Controller
	- Stores the Model data
	- Associates a View to the request
		Can be a physical View implementation or a logical View name
	- The ModelAndView class is simply a container by which the model may be transported to and exposed by the view.
		It is not the model itself

⚪ ViewResolver:
	- Used to map logical View names to actual View implementations

⚪ HandlerMapping
	- Strategy interface used by DispatcherServlet
	- for mapping incoming requests to individual Controllers 
