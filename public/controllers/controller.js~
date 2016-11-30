var myApp = angular.module('myApp', []);
myApp.controller('AppCtrl', ['$scope', '$http', 
			     function($scope, $http){

				 var refresh = function(){
				     $http.get('/resume').success(function(response){
					 console.log("got data!");
					 $scope.resume = response;
				     });
				     
				 };
				 refresh();

// 				 $scope.addContact = function(){
// 				     console.log("entry: " + $scope.contact);
// 				     $http.post('/resume', $scope.contact).success(function(response){
// 					 console.log(response);
// 					 refresh();
// 				     });
// 				 };
				 
// 				 $scope.remove = function(id){
// 				     console.log(id);
// 				     $http.delete('/contactList/' + id).success(function(response){
// 					 refresh();
// 				     });
// 				 };
				 
// 				 $scope.edit = function(id){
// 				     console.log(id);
// 				     $http.get('/contactList/' + id).success(function(response){
// 					 $scope.contact = response;
// 				     });
// 				 };

// 				 $scope.update = function(){
// 				     console.log($scope.contact._id);
// 				     $http.put('/contactList/' + $scope.contact._id, $scope.contact).success(function(response){
// 					 refresh();
// 				     });
// 				 };
				 
				 $scope.deselect = function(){
				     $scope.person = "";
				 };
				 
			     }]);