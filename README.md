# Bootstrap-Modal


```
<style>
    .modal {
        width: 400px;
        position: relative;
        border: 1px solid gray;   
        top: 10px;
        right: 100px;
    }

    .modal-backdrop {
        display: none;
    }
    
</style>

<script src="https://code.jquery.com/jquery-1.12.4.min.js"
        integrity="sha256-ZosEbRLbNQzLpnKIkEdrPv7lOy9C27hHQ+Xp8a4MxAQ="
        crossorigin="anonymous"></script>


<script type="text/javascript">

    $(document).ready(function () {
        $(".popup").hover(function () {

            $("#title").text("this is test");

            $('.modal').modal({
                show: true
            });
        }, function () {
            $('.modal').modal('hide');
        });
    });

</script>

<div><br /></div>

<button class="popup" id="test">Test</button>

<!-- Modal -->
<div class="modal fade" id="myModal" role="dialog">
    <div class="modal-dialog">

        <!-- Modal content-->
        <div class="modal-content alert">
            <div class="modal-header">                
                <h4 class="modal-title" id="title"></h4>
            </div>
            <div class="modal-body">
                <p></p>
            </div>
            <div class="modal-footer">
                <button type="button" class="btn btn-default" data-dismiss="modal">Close</button>
            </div>
        </div>

    </div>
</div>

```




  
