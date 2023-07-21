1. 1 Fancybox modal popup:
   <div class="mb-2">
                                                <a data-fancybox data-src="#north" href="javascript:;">
                                                    <span
                                                        class="text-fz-15-lh-18 fw-400 text-color-2494D1 text-uppercase">
                                                        {!! __('North') !!}
                                                    </span>
                                                </a>
                                                <div class="hidden-office" id="north">
                                                    <div class="position-office">
                                                    <div class="boder-office">
                                                        <div class="img-office">
                                                            <img class="img-fluid w-100"
                                                                 src="{{ rvMedia::getImageUrl(theme_option('name_north')) }}"
                                                                 alt="">
                                                        </div>
                                                        <div class="info-office">
                                                            <h3 class="text-fz-35-lh-41-office fw-400 text-color-1B9948 text-center">
                                                                {!! theme_option('text_north') !!}
                                                            </h3>
                                                            <ul class="hidden-office-list">
                                                                @if(!blank($norths))
                                                                    @foreach($norths as $north)
                                                                        <li>
                                                                            <div>
                                                                                <i class="fas fa-map-marker-alt mr-2 text-color-1B9948"></i>
                                                                                <span
                                                                                    class="text-fz-17-lh-20 fw-400 text-color-000000 pl-2">
                                                                                    {!! $north->address !!}
                                                                                </span>
                                                                            </div>
                                                                            <div>
                                                                                <i class="fas fa-phone-alt mr-2 text-color-1B9948"></i>
                                                                                <span
                                                                                    class="text-fz-17-lh-20 fw-300 text-color-000000 pl-2">
                                                                                    {!! $north->phones !!}
                                                                                </span>
                                                                            </div>
                                                                            <hr>
                                                                        </li>
                                                                    @endforeach
                                                                @endif
                                                            </ul>
                                                        </div>
                                                    </div>
                                                    </div>
                                                </div>
                                            </div>
